# 📖Intro
Artikel ini membahas pembangunan teknologi Ubiquitous Computing dengan tema Penggunaan Teknologi Face Recognition dalam Mencatat Kehadiran Siswa melalui CCTV.
# 💡Latar Belakang
Pendidikan adalah salah satu fondasi pembangunan masyarakat dan negara. Kehadiran siswa di ruang kelas adalah aspek penting dalam mencapai tujuan pendidikan. Kehadiran yang konsisten di kelas memungkinkan siswa untuk mendapatkan manfaat maksimal dari proses pembelajaran, meningkatkan pemahaman, dan mencapai prestasi akademis yang lebih baik. Di sisi lain, dalam konteks penilaian kinerja dan pemantauan kualitas, kehadiran mahasiswa di kelas setiap hari menjadi faktor yang sangat penting [[1](https://www.sciencedirect.com/science/article/pii/S1877050921019232#cebibsec1)].

Namun, pengelolaan kehadiran siswa sering kali melibatkan proses manual yang memakan waktu dan rentan terhadap kesalahan manusia. Pengambilan kehadiran konvensional dengan daftar hadir yang ditandatangani oleh siswa atau melalui pencatatan manual oleh guru memunculkan potensi kesalahan dalam mencatat atau memanipulasi data kehadiran. Pentingnya kehadiran kelas di universitas adalah untuk memantau perkembangan setiap mahasiswa, sehingga pengumpulan data kehadiran tidak boleh salah atau manipulatif [[2](https://www.sciencedirect.com/science/article/pii/S187705092202186X#bbib0001)].

Pada saat yang sama, teknologi pengenalan wajah (face recognition) telah mengalami perkembangan pesat dalam beberapa tahun terakhir. Teknologi ini mampu mendeteksi, melacak, mengidentifikasi, dan memverifikasi wajah manusia dalam gambar atau video yang dihasilkan menggunakan kamera digital [[3](https://www.sciencedirect.com/science/article/pii/S2590005619300141)]. Dengan teknologi ini, kita dapat mencapai pencatatan kehadiran yang lebih akurat dan efisien. Dalam rangka mengurangi kesalahan manusia yang sering terjadi dalam proses pengambilan kehadiran konvensional, sistem kehadiran otomatis telah direncanakan untuk memvalidasi efisiensi algoritma face recognition yang diusulkan [[4](https://ieeexplore.ieee.org/document/8721062)].

Proyek "Penggunaan Teknologi Face Recognition dalam Mencatat Kehadiran Siswa melalui CCTV" bertujuan untuk mengintegrasikan teknologi pengenalan wajah (Face Recognition) sebagai solusi otomatis dalam mencatat kehadiran siswa. Proyek ini akan memanfaatkan CCTV yang sudah umum digunakan di lembaga pendidikan untuk mengidentifikasi siswa secara otomatis saat mereka memasuki ruang kelas. Dengan penggunaan teknologi ini, diharapkan dapat mengurangi kesalahan manusia, meningkatkan akurasi pencatatan kehadiran, dan meminimalkan risiko manipulasi data kehadiran.

Proyek ini juga sejalan dengan upaya untuk menciptakan ruang kelas cerdas (smart class) yang dapat memberikan manfaat lebih lanjut bagi lembaga pendidikan. Selain memudahkan pengelolaan kehadiran siswa, teknologi ini juga membantu menciptakan lingkungan pembelajaran yang lebih modern, efisien, dan terkini.

Dengan pengintegrasian teknologi Face Recognition dalam pencatatan kehadiran siswa, proyek ini diharapkan dapat memberikan kontribusi positif dalam mengelola kehadiran siswa di lingkungan pendidikan, meminimalkan potensi kesalahan, dan membuka jalan menuju pendidikan yang lebih efisien serta berkualitas.
# 🌻Branding
- Merk (Brand): FaceRoom CCTV
- Inspirasi Merk: Teknologi pengenalan wajah (face recognition), yang membantu mengawasi dan memantau kehadiran siswa di ruangan (room) menggunakan angle gambar CCTV.
- Tagline: "CCTV Pintar Pendeteksi Kehadiran Siswa" / “Menghadirkan Teknologi Pendeteksi Kehadiran untuk CCTV”
- Campaign (Kampanye): Teknologi face recognition memudahkan siswa, orang tua dan pengajar. Tidak perlu lagi kartu identitas fisik atau proses check-in manual. Cukup hadir di kelas dan kami yang mengurus sisanya. Kami memberikan pengalaman yang lebih nyaman bagi semua yang terlibat. Orangtua siswa tidak perlu khawatir lagi dalam memastikan apakah anak nya pasti hadir di kelas atau tidak.
- Target User (Pengguna Sasaran): Pihak orangtua, sekolah, perguruan tinggi, dan institusi pendidikan lainnya yang ingin memantau kehadiran siswa secara akurat dan efisien.

- User Experience Theme (Tema Pengalaman Pengguna):
  - Antarmuka yang ramah pengguna dan mudah digunakan untuk pengelolaan kehadiran, serta kemampuan untuk mengakses data kehadiran melalui aplikasi berbasis mobile untuk memantau kehadiran dengan mudah.
  - Menghilangkan presensi kehadiran secara manual (memanggil / memeriksa murid satu per satu oleh guru)
  - Orangtua tidak perlu mengontak guru untuk memastikan kehadiran anak nya. Orangtua langsung menerima pesan whatsapp / telegram laporan hasil kehadiran dari chat bot.
# 🎯User Story
|Sebagai|Saya ingin bisa|Sehingga|Prioritas|
|--|--|--|--|
|Sistem|Merekognisi wajah peserta|Bisa mencatat status hadir dan tidak hadir dari seluruh peserta|⭐⭐⭐⭐⭐|
|Sistem|Membuat & Mengirim data laporan kehadiran seluruh peserta|Bisa memberi tahu orang tua / wali mengenai laporan kehadiran|⭐⭐⭐⭐|
|Sistem|Menangkap gambar dari CCTV secara terjadwal|Bisa menjadikan hasil tangkapan gambar sebagai bahan untuk face recognition|⭐⭐⭐|
|Sistem|Menyajikan interface yang menarik untuk client android app|Bisa memaksimalkan kenyamanan pengguna|⭐
# 📚Metode dan Algoritma
- Sensor
  - Face recognition : MTCNN
- Kamera : CCTV
- Responder
  - Telegram bot
- Mobile software development
  - Agile
# 🌲Struktur Data
<div>
<img src="https://lh7-us.googleusercontent.com/jDTReG4dHdIvGCkh4822mt0ZMvfKvu40MwyJ2TVcrbwcrpJDNNaiGe0pPz8wFjv2JmFTvQrWyBjPdUL9ZR_cbW9_2Gv2cWM3bWT17nGfHeL7NEkt8hjKFvmC-qltA4Bu5Ilib1IsHuOKJesjci7Mpiw" alt="drawing" width="700"/>
</div>

1. Image dicapture
2. Dicatat di table attendance siapa hadir siapa tidak
3. Dibuat laporan per mahasiswa di report_message, untuk nanti dikirim message nya ke ortu / wali
# 🏗Arsitektur Sistem
<div><img src="https://lh7-us.googleusercontent.com/kvzAZwx2C_YgAwKeei665ho8HpahgEfLRElUEEgElKwaervUP11s6XR_0LAVNaJANZ-yuyZ1DGF7-26KbZGLLPw7omOdxgE2E2_vEtWgELs0RIZDlIKMLhnK50XuBodAz4qp5kYDx0tor-bZnZZp-fM" alt="drawing" width="700" /></div>

# 💻Deskripsi Teknologi
- Mesin Komputasi
  - Cloud server : Google Cloud Platform - Cloud Run
Salah satu layanan komputasi yang disediakan oleh Google Cloud Platform untuk menjalankan aplikasi dalam bentuk container. Mendukung Continuous Integration/Continuous Deployment (CI/CD) untuk mempermudah proses pengembangan aplikasi.
  - Smartphone : Android (vivo Y21)
Aplikasi client mobile “FaceRoom CCTV” nantinya bisa dipakai sebagai perantara antara CCTV dengan cloud server. Akan running di background untuk melakukan penangkapan gambar dan pengiriman gambar ke server pada jadwal yang ditentukan.
- Software Development
  - Mobile development : Flutter untuk Android
Flutter adalah sebuah framework yang memungkinkan pengembang untuk membuat aplikasi lintas platform (cross-platform) dengan lebih mudah, termasuk aplikasi untuk Android. Karena Android adalah platform yang sangat luas digunakan saat ini, diharapkan bahwa FaceRoom CCTV dapat menjangkau sebagian besar masyarakat.
  - Backend development : FastAPI
FastAPI adalah sebuah framework Python yang dirancang untuk mempermudah pengembang dalam pembuatan REST API dengan menggunakan bahasa pemrograman Python. Pemilihan Python sebagai bahasa pemrograman untuk REST API bertujuan untuk memudahkan integrasi dengan model Face Recognition yang digunakan dalam proyek ini.
- Sensor : CCTV
- Responder : Smartphone yang terpasang Telegram atau WhatsApp dianggap sebagai perangkat yang berperan sebagai responder. Perangkat ini memberikan respon pesan untuk orang tua / wali mengenai laporan kehadiran yang dihasilkan oleh proses face recognition.
# User Experience (UX) Design
<div><img src="https://lh7-us.googleusercontent.com/7flPxfA6j1E_B62ZsNZtKbSxsIaCNdhGsXIClhT1FXhdyvUCh2ynkyqvBYGfO4MH3nlbJwCzEyGtNEr2FHRHZ1ZMYEoVo2UFi1gGu8Azy84FQjUaun7G3ByP1GI0UFtCOaZDnSRJtMTa_7MovFCx2qg" alt="drawing" width=700 /></div>

https://www.figma.com/file/NAijilNHuOfDDzhSQ0C7PJ/ubigong?type=design&node-id=0%3A1&mode=design&t=wFeALLDqftTj12Qh-1

# Demo fitur running client app di background untuk keperluan schedule penangkapan gambar dan pengiriman ke server
<div>
  <img src="https://github.com/tegar-anggana/faceroom_cctv/assets/80917799/2d5f157c-291c-4a9e-bb72-5ef06253515e" alt="" width=300 />
  <img src="https://github.com/tegar-anggana/faceroom_cctv/assets/80917799/54d4b5da-68e6-4afe-bdd8-0c924a318611" alt="" width=300 />
</div>
