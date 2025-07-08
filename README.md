## Company Profile Website Generator

Project ini adalah capstone project untuk event IBM x Hacktiv8 Indonesia, yaitu IBM SkillsBuild: Code Generation and Optimization Using IBM Granite.

Python Jupyter Notebook ini merupakan workflow generator otomatis untuk membuat landing page sebuah company profile menggunakan model AI IBM Granite yang diakses melalui Replicate API. Dengan menggunakan pendekatan one-shot prompting yang diajarkan selama IBM SkillsBuild x Hacktiv8 Indonesia, aplikasi ini dapat menghasilkan file HTML, CSS, dan JavaScript lengkap hanya dari input prompt "company info" dan "industry" dari user dengan template one-shot prompt yang sudah dipersiapkan.

### Jupyter Notebook Workflow:
1. **Instalasi Library & Autentikasi Replicate**  
   Instal library yang dibutuhkan dan lakukan autentikasi dengan Replicate API token (sudah dibuatkan cara dapat tokennya dibawah).
2. **Inisialisasi Model dengan Replicate Model Wrapper**  
   Model IBM Granite diinisialisasi dengan model "ibm-granite/granite-3.3-8b-instruct"
3. **Format One-Shot Prompt**  
   Prompt dibuat secara dinamis menggunakan informasi perusahaan dan satu contoh output.
4. **Generate & Tampilkan Website**  
   Model AI menghasilkan code HTML landing page, yang kemudian dapat langsung ditampilkan dan dievaluasi.
5. **Refined One-Shot Prompt**  
   Workflow ini pun mendukung proses refinement, yaitu mengupdate hasil website menggunakan prompt baru dan one-shot prompt refinement example.

### Langkah-langkah Mendapatkan Replicate API Token:

1. **Daftar atau Login ke Replicate**
   - Buka [https://replicate.com](https://replicate.com) dan lakukan sign up atau login jika sudah punya akun.

2. **Akses Page API Tokens**
   - Setelah login, klik foto profil user di pojok kanan atas lalu pilih **"Account"**.
   - Pada menu sebelah kiri, pilih **"API Tokens"** atau langsung buka [https://replicate.com/account/api-tokens](https://replicate.com/account/api-tokens).

3. **Buat Token Baru**
   - Klik tombol **"Create token"**.
   - Beri nama sesuai keinginan (misal: `capstone-generator`) dan klik **"Create token"**.

4. **Copy and Paste Token**
   - Copy kode token yang dimulai dengan `r8_...` dan **simpan** di tempat aman.
   - Gunakan token ini untuk autentikasi di Jupyter Notebook user.

**Catatan:** Jangan bagikan token ke orang lain. Token ini bersifat rahasia dan digunakan untuk mengakses API Replicate milik user pribadi.
