# Kerangka Riset Investasi Kripto Jangka Panjang (Invest & Hold Framework)

Dokumen ini merupakan panduan riset fundamental komprehensif untuk mengevaluasi proyek kripto/blockchain dalam jangka panjang (*Invest & Hold*). Kerangka kerja ini menyintesis seluruh dimensi teknis, ekonomi, pasar, tim, hingga risiko keamanan guna membedakan proyek berbobot tinggi (*blue-chip/high-utility*) dari proyek spekulatif berbasis *hype*.

---

## 1. Problem-Solution Fit & Lanskap Kompetitif (The "Moat")

Teknologi hebat tidak berguna jika tidak memiliki kegunaan nyata dan keunggulan kompetitif yang bertahan lama.

* **Problem-Solution Fit:**
  * Apakah proyek ini menyelesaikan masalah nyata di dunia nyata atau di ekosistem blockchain (misal: skalabilitas, abstraksi kompleksitas, interoperabilitas)?
  * Seberapa krusial masalah tersebut dan seberapa besar permintaan (*demand*) terhadap solusinya?
* **Unique Selling Point (USP):**
  * Apa nilai unik utama yang dimiliki proyek yang tidak dimiliki oleh Ethereum, Solana, atau kompetitor langsung lainnya?
* **Network Effect:**
  * Apakah proyek memiliki keunggulan sebagai *First Mover*, atau ekosistem yang mampu mengunci (*lock-in*) loyalitas pengguna dan pengembang sehingga sulit berpindah platform?
* **Analisis Kompetitor Langsung (Direct Competitors):**
  * Siapa 3 kompetitor utama? Apa keunggulan dan kelemahan teknis proyek ini dibanding mereka (misal: Solana vs Aptos, Uniswap vs Jupiter, Monolithic vs Sharding)?
* **Barriers to Entry (Hambatan Masuk):**
  * Seberapa sulit bagi pemain baru untuk meniru kode, arsitektur, atau jaringan proyek ini?
* **Kemitraan Strategis (Strategic Partnerships):**
  * Apakah ada integrasi dan kemitraan dunia nyata dengan perusahaan besar (seperti Google Cloud, AWS, Visa) atau protokol Web3 yang kredibel?

### *Sub-kategori Tambahan untuk DeFi / App-Chain:*
* **Mekanisme Yield:** Apakah imbal hasil (*yield*) berasal dari *real revenue* (biaya transaksi/trading riil) atau sekadar dari emisi inflasi token?
* **Ekosistem Pengembang Eksternal (External Builders):** Berapa banyak tim pihak ketiga yang membangun dApps/infrastruktur (seperti *vault* otomatis, *lending*) di atas rantai ini?

---

## 2. Analisis Teknologi & Infrastruktur (Technology Analysis)

Evaluasi kelayakan arsitektur sistem, keandalan, dan skalabilitas teknis.

* **Tech Stack & Bahasa Pemrograman:**
  * Bahasa dan *framework* apa yang digunakan (Rust, Solidity, Move, WASM)? Seberapa mudah dan aman bagi pengembang untuk membangun dApps di atasnya?
* **Mekanisme Konsensus & Algoritma:**
  * Bagaimana jaringan mencapai kesepakatan (PoS, Dynamic Sharding, DAG, BFT)? Bagaimanakah keandalan dan arsitekturnya?
* **Kecepatan & Skalabilitas (Speed & Scale):**
  * Berapa throughput riil (TPS) dan waktu finalitas (*finality time*) transaksi?
* **Interoperabilitas (Cross-Chain):**
  * Apakah teknologi ini dapat berkomunikasi dengan rantai lain secara native (misal: via Chain Signatures, Rainbow Bridge, LayerZero, IBC), atau terisolasi dalam *silo*?
* **Status Open Source & Ketahanan Jaringan (Uptime & Liveness):**
  * Apakah kodenya dapat diverifikasi publik? Bagaimana rekam jejak *uptime* jaringan (pernah mengalami *downtime* atau rentan terhadap serangan *spam*)?

### *Sub-kategori Tambahan untuk App-Chain / DEX (misal: CLOB):*
* **Performa Latensi:** Seberapa cepat konfirmasi transaksi dibandingkan kompetitor CLOB (Central Limit Order Book) lain?
* **Ketergantungan Oracle:** Bagaimana proyek mendapatkan data harga? Menggunakan oracle internal atau penyedia pihak ketiga (Pyth, Chainlink)?

---

## 3. Analisis Pasar & Likuiditas (Market Analysis)

Menilai valuasi, struktur pemegang token, dan risiko likuiditas di bursa.

* **Market Cap vs. Fully Diluted Valuation (FDV):**
  * Berapa Market Cap (sirkulasi berjalan) dibanding FDV (total suplai penuh)? 
  * *Perhatian:* Jika $MC = \$1\text{B}$ sedangkan $FDV = \$10\text{B}$, terdapat gap besar yang menandakan potensi tekanan jual tinggi di masa depan akibat *unlock* token.
* **Konsentrasi Pemegang Token (Whale Watch):**
  * Berapa persen suplai yang dikuasai oleh 10-100 dompet teratas? Jika $> 50\%$, ada risiko manipulasi harga oleh segelintir *Whale*.
* **Kualitas Listing & Ketersediaan Bursa:**
  * Apakah token terdaftar di CEX Tier-1 (Binance, Coinbase, Kraken, OKX) atau hanya di DEX berlikuiditas rendah?
* **Kedalaman Likuiditas (Liquidity Depth):**
  * Seberapa dalam *2% market depth* di bursa utama? Apakah investor institusi/ritel dapat masuk dan keluar posisi tanpa menyebabkan *slippage* besar?
* **Sentimen Pasar & Kualitas Komunitas:**
  * Apakah diskusi di Twitter/Discord didominasi oleh pembahasan teknis & adopsi organik, atau hanya *bot spam* yang berteriak *"to the moon"*?

---

## 4. Tokenomics & Keberlanjutan Ekonomi (Economic Model)

Merupakan "kebijakan moneter" proyek yang menentukan nilai jangka panjang token.

* **Fungsi & Kegunaan Token (Token Utility):**
  * Untuk apa token digunakan (Staking/Keamanan, Biaya Gas, Governance, Storage Staking)?
* **Jadwal Vesting & Cliff (Vesting Schedule):**
  * Kapan token milik investor awal (VC) dan tim akan dibuka (*unlocked*)? Kenaikan suplai mendadak (*cliff unlock*) sering memicu *price dump*.
* **Mekanisme Inflasi vs. Deflasi (Burn Mechanism):**
  * Berapa tingkat inflasi tahunan? Apakah ada mekanisme pembakaran token (*fee burn* seperti EIP-1559) yang membuat token menjadi langka seiring peningkatan penggunaan?
* **Model Pendapatan & Pengelolaan Kas (Treasury Runway):**
  * Dari mana protokol menghasilkan pemasukan riil? Apakah kas (*treasury*) proyek cukup untuk membiayai operasional dan pengembang selama 3–5 tahun kondisi pasar lesu (*Bear Market*)?
* **Cadangan Asuransi (Insurance Fund) & Net Flow:**
  * Apakah ada dana asuransi untuk menahan volatilitas ekstrem (mencegah *bad debt*)? Apakah aliran uang masuk (*net flow*) lebih besar dari emisi reward token?

---

## 5. Tim, Investor & Modal Sosial (The "Who" Behind the Code)

Dunia kripto bersifat *open-source*, sehingga reputasi dan eksekusi tim menjadi benteng pembeda utama.

* **Rekam Jejak Pendiri & Tim (Founders' Track Record):**
  * Siapa pendirinya? Apakah identitas mereka terbuka (*doxxed*) atau anonim? Apakah mereka memiliki riwayat sukses atau pernah terlibat skandal/kegagalan di proyek sebelumnya?
* **Kualitas Investor Utama / Venture Capital (VC Tier 1):**
  * Siapa pemodal awal (*seed round*)? Dukungan dari VC Tier-1 (seperti a16z, Paradigm, Sequoia, Polychain, Binance Labs) menandakan *due diligence* ketat telah dilakukan.
* **Aktivitas Pengembang (Developer Activity):**
  * Bagaimana statistik GitHub proyek? Apakah terdapat komit (*commits*) dan pengembang aktif mingguan yang konsisten, atau proyek sudah menjadi "kota hantu"?
* **Penasihat (Advisors) & Tokoh Industri:**
  * Siapa pakar atau akademisi yang mendampingi pengembangan proyek?

---

## 6. Eksekusi, Roadmap & Katalis (The "When")

Menilai rekam jejak eksekusi tim dalam memenuhi janji pengembangan.

* **Riwayat Milestone (Milestone History):**
  * Apakah tim selalu mencapai target *roadmap* tepat waktu? Penundaan berulang (*frequent delays*) merupakan *red flag* utama.
* **Katalis Masa Depan (Future Catalysts):**
  * Peristiwa besar apa yang akan terjadi dalam 6–12 bulan ke depan (misal: *Mainnet launch*, *Halving*, *Upgrade* arsitektur besar, *Rebranding*, pengajuan ETF)?

---

## 7. Keamanan, Risiko & Regulasi (The "Safety Net")

Mengidentifikasi titik lemah fatal yang dapat menghancurkan proyek.

* **Audit Keamanan Smart Contract:**
  * Apakah kode telah diaudit oleh firma keamanan independen ternama (seperti OpenZeppelin, CertiK, Hacken, Trail of Bits, Spearbit)?
* **Risiko Sentralisasi & Admin Keys:**
  * Seberapa besar kendali tim melalui *admin keys*? Bisakah mereka melakukan *upgrade* kontrak secara sepihak yang berisiko *rugpull*?
* **Risiko Regulasi (SEC & Global):**
  * Berapa besar risiko token dikategorikan sebagai *security* (efek berharga) oleh SEC atau badan regulasi keuangan dunia?

---

## 8. Tabel Matriks Skoring Cepat (Quick-Reference Matrix)

Gunakan tabel ini untuk memberi skor (1–10) atau penilaian cepat pada proyek:

| Parameter Riset | Indikator Positif (*Bullish*) | Indikator Negatif / *Red Flag* (*Bearish*) |
| :--- | :--- | :--- |
| **Kualitas VC / Investor** | Didukung VC Tier-1 (a16z, Paradigm, Sequoia, dll.) | Tidak ada VC atau didukung pemodal tidak dikenal |
| **Aktivitas Kode (GitHub)** | Komit harian/mingguan aktif dari banyak kontributor | Tidak ada pembaharuan kode > 3 bulan |
| **Audit Keamanan** | Ter-audit berlapis oleh firma ternama (OpenZeppelin/Hacken) | Belum diaudit atau menggunakan auditor abal-abal |
| **Laju Inflasi & Tokenomics** | Terukur, melandai, atau memiliki mekanisme pembakaran (*deflasioner*) | Emisi token tanpa batas / inflasi sangat tinggi |
| **Struktur Pemegang Token** | Terdistribusi luas di komunitas ritel & institusi | Terkonsentrasi pada segelintir dompet *Whale* (>50%) |
| **Model Pendapatan (Revenue)** | Menghasilkan *real yield* dari biaya transaksi riil | Bergantung 100% pada pencetakan token baru |
| **Rasio Staking** | Tinggi (>40% sirkulasi terkunci dalam staking) | Sangat rendah (<10%), berisiko *dump* mendadak |

---

## 9. Pertanyaan Kunci Penentu (*The Killer Question*)

Sebelum mengambil keputusan investasi jangka panjang pada suatu proyek, jawab pertanyaan kritis ini:

> **"Jika proyek ini gagal dalam 2 tahun ke depan, apa alasan yang paling memungkinkan?"**
> *(Apakah karena regulasi, tekanan jual vesting VC, kelemahan sharding/konsensus, atau kompetisi dari rantai lain?)*

---

## 10. Studi Kasus Implementasi: Analisis Fundamental NEAR Protocol

Berikut adalah contoh penerapan kerangka riset ini pada **NEAR Protocol**:

### 1. Competitive Landscape (Moat)
* **Problem-Solution Fit:** Mengatasi hambatan adopsi Web3 (*User Experience/UX*). Menggunakan *Named Accounts* (seperti `budi.near`) sehingga pengguna tidak perlu mengingat alamat heksadesimal yang rumit.
* **USP:** *Chain Abstraction* (memungkinkan 1 akun NEAR bertransaksi di 35+ rantai lain) dan *User-Owned AI* (infrastruktur AI terdesentralisasi).
* **Network Effect:** Identitas akun terikat pada ekosistem NEAR.
* **Competitor Benchmarking:** Solana unggul dalam eksekusi monolitik cepat, sedangkan NEAR menggunakan skalabilitas horisontal (*Nightshade Sharding*). NEAR bertindak sebagai *Chain Abstraction Layer* untuk semua L1/L2.

### 2. Technology Analysis
* **Tech Stack:** Menggunakan WebAssembly (WASM) yang mendukung bahasa populer seperti Rust dan JavaScript/TypeScript.
* **Mekanisme Konsensus:** Nightshade Sharding + Doomslug. Telah mengimplementasikan *Stateless Validation* (menurunkan syarat perangkat keras validator).
* **Speed & Scale:** Menguji kemampuan hingga 1.000.000 TPS dengan 70+ *shards* dan finalitas ~1,2 detik.
* **Interoperability:** Sangat kuat melalui *Chain Signatures*, *Rainbow Bridge*, dan integrasi LayerZero.

### 3. Market Analysis
* **FDV vs Market Cap:** Suplai awal genesis (1 miliar token) telah sepenuhnya *unlocked*. Gap Market Cap dan FDV sangat kecil, menekan risiko inflasi investor awal.
* **Likuiditas & Listing:** Terdaftar di seluruh CEX Tier-1 (Binance, Coinbase, Kraken) dan didukung ETP Institusional (Bitwise Staking ETP).

### 4. Tokenomics
* **Burn Mechanism:** 70% biaya gas dibakar secara permanen, 30% diberikan kepada pengembang *smart contract*.
* **Deflasi:** Laju inflasi diturunkan dari 5% menjadi 2.5% (*Halving Upgrade*). Penggunaan AI agents & *intents* berpotensi membuat token deflasioner.
* **Treasury Runway:** NEAR Foundation memiliki dana cadangan ratusan juta USD (stablecoin & NEAR) yang cukup membiayai operasional hingga 5 tahun ke depan.

### 5. Team & Social Capital
* **Founders:** Illia Polosukhin (salah satu penulis utama paper Google *"Attention Is All You Need"* yang melahirkan Transformer/ChatGPT) dan Alexander Skidanov (ex-MemSQL).
* **Dev Activity:** Konsisten masuk dalam 5 besar proyek dengan komit GitHub terbanyak (Laporan Electric Capital).

### 6. Execution & Roadmap
* **Catalyst:** Peluncuran *Agentic Web* (eksekusi perintah transaksi on-chain otomatis oleh AI Agent).

### 7. Security & Risk
* **Audit:** Diaudit oleh Hacken, BlockSec, Halborn, dan Sigma Prime.
* **Risiko Sentralisasi:** Mitigasi melalui *Stateless Validation* dan pembubaran Pagoda menuju *House of Stake* (tata kelola terdesentralisasi).

### *Killer Question untuk NEAR Protocol:*
> *"Jika Solana berhasil melakukan scaling tanpa sharding dan Ethereum L2 menjadi sangat murah via EIP-4844, apakah pengguna masih membutuhkan Chain Abstraction milik NEAR?"*  
> **Jawaban Riset:** Butuh, karena *Chain Abstraction* menyembunyikan kompleksitas transaksi lintas rantai (bukan sekadar biaya *gas* murah), terutama untuk transaksi mandiri oleh AI Agent (*Agentic Web*).
