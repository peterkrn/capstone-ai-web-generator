## Company Profile Website Generator

Proyek ini adalah capstone project IBM SkillsBuild: Code Generation and Optimization Using IBM Granite, collaborating with Hacktiv8 Indonesia. 

Python Notebook ini adalah generator otomatis Company Profile landing page menggunakan model AI IBM Granite yang diakses melalui Replicate API. Dengan menggunakan pendekatan one-shot prompting yang diajarkan selama IBM SkillsBuild x Hacktiv8 Indonesia, aplikasi ini dapat menghasilkan file HTML, CSS, dan JavaScript lengkap hanya dari input informasi perusahaan serta contoh output yang sudah tersedia.

### Alur Kerja Utama:
1. **Instalasi Library & Autentikasi Replicate**  
   Instal library yang dibutuhkan dan lakukan autentikasi dengan Replicate API token.
2. **Inisialisasi Model dengan Replicate Model Wrapper**  
   Model IBM Granite diinisialisasi agar bisa menerima prompt dan menghasilkan kode HTML/CSS.
3. **Format One-Shot Prompt**  
   Prompt dibuat secara dinamis menggunakan informasi perusahaan dan satu contoh output.
4. **Generate & Tampilkan Website**  
   Model AI menghasilkan kode website, yang kemudian dapat langsung ditampilkan dan dievaluasi.
5. **Refined One-Shot Prompt**  
   Aplikasi juga mendukung proses refinement, yaitu memperbaiki/mengupdate hasil website menggunakan prompt baru dan contoh perubahan.

Dengan workflow ini, Anda dapat membuat website profil perusahaan hanya dalam beberapa detik, cukup dengan mengisi input dan menekan tombol Run!

### Langkah-langkah Mendapatkan Replicate API Token:

1. **Daftar atau Login ke Replicate**
   - Buka [https://replicate.com](https://replicate.com) dan lakukan registrasi (sign up) atau login jika sudah punya akun.

2. **Akses Halaman API Tokens**
   - Setelah login, klik foto profil Anda di pojok kanan atas lalu pilih **"Account"**.
   - Pada menu sebelah kiri, pilih **"API Tokens"** atau langsung buka [https://replicate.com/account/api-tokens](https://replicate.com/account/api-tokens).

3. **Buat Token Baru**
   - Klik tombol **"Create token"**.
   - Beri nama sesuai keinginan (misal: `capstone-generator`) dan klik **"Create token"**.

4. **Salin Token**
   - Salin kode token yang dimulai dengan `r8_...` dan **simpan** di tempat aman.
   - Gunakan token ini untuk autentikasi di aplikasi notebook Anda.

**Catatan:** Jangan bagikan token ke orang lain. Token ini bersifat rahasia dan digunakan untuk mengakses layanan API Replicate dari notebook.
