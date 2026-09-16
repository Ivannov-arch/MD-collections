**Ya, LLM masih menggunakan *cosine similarity*, tetapi penggunaannya terbatas pada area spesifik seperti pemrosesan embedding.**

Model tidak memakai *cosine similarity* sebagai mekanisme utama saat menghasilkan kata demi kata (*generation*).

---

### Di Mana *Cosine Similarity* Digunakan?

* **Retrieval-Augmented Generation (RAG) & Vector Database:**
Saat membuat sistem RAG, dokumen referensi disimpan dalam bentuk *vector embedding*. Ketika user memberikan pertanyaan, sistem menghitung *cosine similarity* antara vektor pertanyaan dan vektor dokumen untuk menemukan informasi paling relevan.
* **Semantic Search & Clustering:**
Digunakan untuk mengukur seberapa mirip makna antar dua teks, kalimat, atau dokumen tanpa memperhatikan panjang teksnya.
* **Evaluasi Model & Clustering Embedding:**
Digunakan oleh peneliti untuk membandingkan ruang representasi (*embedding space*) antar model atau mengelompokkan topik.

---

### Mengapa Bukan *Cosine Similarity* Utama di Dalam LLM?

Arsitektur utama LLM (Transformer) menggunakan mekanisme **Scaled Dot-Product Attention**:

$$\text{Attention}(Q, K, V) = \text{softmax}\left(\frac{QK^T}{\sqrt{d_k}}\right)V$$

Perbedaan utamanya dibanding *cosine similarity*:

| Fitur | Cosine Similarity | Dot Product (Di dalam LLM) |
| --- | --- | --- |
| **Formula** | $\frac{A \cdot B}{\Vert{}A\Vert{} \Vert{}B\Vert{}}$ | $A \cdot B$ |
| **Normalisasi Vektor** | Membagi dengan panjang (magnitudo) vektor. | Tidak membagi panjang vektor. |
| **Pengaruh Magnitudo** | Membuang informasi panjang vektor. | Mempertahankan magnitudo sebagai indikator tingkat keyakinan (*confidence/importance*). |

Pada mekanisme *Self-Attention*, magnitudo vektor membawa informasi penting tentang seberapa kuat pengaruh suatu kata (*token*) terhadap token lainnya. Jika dibagi dengan panjang vektornya seperti pada *cosine similarity*, informasi penting tersebut justru akan hilang.

---

*Cosine similarity* berperan besar di **luar** LLM (seperti pencarian dokumen dan RAG), sementara di **dalam** LLM itu sendiri, yang digunakan adalah *dot product* biasa.