Berikut adalah panduan pengisian formulir konfigurasi **Google Auth** yang sedang Anda buka:

1. **Enable Sign in with Google**
* Centang (*check*) kotak ini untuk mengaktifkan login Google.


2. **Client IDs**
* Isi dengan **Client ID** yang didapat dari **Google Cloud Console**.
* Catatan: Input saat ini (`admin@xmu.edu.my`) **salah**. Client ID dari Google biasanya berbentuk string panjang yang diakhiri dengan `.apps.googleusercontent.com` (contoh: `123456789012-abc123def456.apps.googleusercontent.com`).


3. **Client Secret (for OAuth)**
* Isi dengan **Client Secret** yang dibuat bersamaan dengan Client ID di Google Cloud Console.


4. **Skip nonce checks & Allow users without an email**
* Biarkan **kosong / tidak dicentang** (*default*), kecuali Anda memiliki kebutuhan khusus untuk aplikasi mobile (iOS) atau skenario tertentu.


5. **Callback URL (for OAuth)**
* **Tidak perlu diisi/diubah**, tetapi **salin (copy)** URL ini (`[https://cfelrulptrlqqnusnlaq.supabase.co/auth/v1/callback](https://cfelrulptrlqqnusnlaq.supabase.co/auth/v1/callback)`) dan tempelkan ke kolom **Authorized redirect URIs** pada pengaturan OAuth Credentials di **Google Cloud Console**.



---

### Cara Mendapatkan Client ID & Client Secret:

1. Buka Google Cloud Console.
2. Buat proyek baru atau pilih proyek yang ada.
3. Buka menu **APIs & Services** > **OAuth consent screen**, lalu ikuti alur konfigurasinya (*External* / *Internal*).
4. Masuk ke **APIs & Services** > **Credentials**.
5. Klik **Create Credentials** > **OAuth client ID**.
6. Pilih **Web application**, lalu masukkan Callback URL dari Supabase ke bagian **Authorized redirect URIs**.
7. Setelah dibuat, Anda akan mendapatkan **Client ID** dan **Client Secret** untuk dimasukkan ke Supabase.

Setelah semua diisi dengan benar, klik tombol **Save** di bagian bawah.

Berikut adalah panduan pengisian formulir konfigurasi **Google Auth** yang sedang Anda buka:

1. **Enable Sign in with Google**
* Centang (*check*) kotak ini untuk mengaktifkan login Google.


2. **Client IDs**
* Isi dengan **Client ID** yang didapat dari **Google Cloud Console**.
* Catatan: Input saat ini (`admin@xmu.edu.my`) **salah**. Client ID dari Google biasanya berbentuk string panjang yang diakhiri dengan `.apps.googleusercontent.com` (contoh: `123456789012-abc123def456.apps.googleusercontent.com`).


3. **Client Secret (for OAuth)**
* Isi dengan **Client Secret** yang dibuat bersamaan dengan Client ID di Google Cloud Console.


4. **Skip nonce checks & Allow users without an email**
* Biarkan **kosong / tidak dicentang** (*default*), kecuali Anda memiliki kebutuhan khusus untuk aplikasi mobile (iOS) atau skenario tertentu.


5. **Callback URL (for OAuth)**
* **Tidak perlu diisi/diubah**, tetapi **salin (copy)** URL ini (`[https://cfelrulptrlqqnusnlaq.supabase.co/auth/v1/callback](https://cfelrulptrlqqnusnlaq.supabase.co/auth/v1/callback)`) dan tempelkan ke kolom **Authorized redirect URIs** pada pengaturan OAuth Credentials di **Google Cloud Console**.



---

### Cara Mendapatkan Client ID & Client Secret:

1. Buka Google Cloud Console.
2. Buat proyek baru atau pilih proyek yang ada.
3. Buka menu **APIs & Services** > **OAuth consent screen**, lalu ikuti alur konfigurasinya (*External* / *Internal*).
4. Masuk ke **APIs & Services** > **Credentials**.
5. Klik **Create Credentials** > **OAuth client ID**.
6. Pilih **Web application**, lalu masukkan Callback URL dari Supabase ke bagian **Authorized redirect URIs**.
7. Setelah dibuat, Anda akan mendapatkan **Client ID** dan **Client Secret** untuk dimasukkan ke Supabase.

Setelah semua diisi dengan benar, klik tombol **Save** di bagian bawah.