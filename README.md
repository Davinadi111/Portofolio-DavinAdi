<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Portofolio Davin</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #ecf0f1;
    }

    nav {
      background-color: #2c3e50;
      display: flex;
      justify-content: center;
      padding: 15px 0;
    }

    nav button {
      background-color: #3498db;
      color: white;
      border: none;
      padding: 10px 20px;
      margin: 0 10px;
      border-radius: 5px;
      cursor: pointer;
      font-size: 16px;
    }

    nav button:hover {
      background-color: #2980b9;
    }

    .page {
      display: none;
      padding: 30px;
      background-color: white;
      margin: 20px auto;
      max-width: 800px;
      border-radius: 10px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }

    .page.active {
      display: block;
    }

    h1 {
      color: #2c3e50;
    }

    ul {
      padding-left: 20px;
    }

    p, li {
      font-size: 18px;
    }
  </style>
</head>
<body>

  <nav>
    <button onclick="showPage('beranda')">Beranda</button>
    <button onclick="showPage('prestasi')">Prestasi & Pengalaman</button>
    <button onclick="showPage('skill')">Skill</button>
  </nav>

  <div id="beranda" class="page active">
    <h1>Selamat Datang di Portofolio Saya</h1>
    <p><strong>Nama:</strong> Davin Adi Faringga</p>
    <p><strong>Alamat:</strong> Silirbaru, Pesanggaran, Banyuwangi</p>
    <p><strong>Umur:</strong> 16 Tahun</p>
    <p><strong>Riwayat Pendidikan:</strong></p>
    <ul>
      <li>TK Pertiwi 5</li>
      <li>SDN 2 Pesanggaran</li>
      <li>SMPN 2 Pesanggaran</li>
      <li>SMAN 1 Pesanggaran</li>
    </ul>
    <p>Saya sangat antusias untuk terus belajar dan berkembang dalam berbagai bidang digital. Semoga portofolio ini menjadi awal dari perjalanan panjang menuju masa depan yang gemilang.</p>
  </div>

  <div id="prestasi" class="page">
    <h1>Prestasi dan Pengalaman</h1>
    <p>Saya pernah menjadi anggota <strong>Paskibra tingkat Kecamatan</strong>, pengalaman yang membentuk kedisiplinan dan rasa cinta tanah air. Selain itu, saya juga pernah dipercaya untuk <strong>menyambut Kepala Pendidikan Cabang Banyuwangi</strong> sebagai pasukan baris-berbaris di SMAN 1 Pesanggaran.</p>
    <p>Pengalaman ini sangat berkesan dan membangun rasa percaya diri serta kemampuan bekerja dalam tim.</p>
  </div>

  <div id="skill" class="page">
    <h1>Skill</h1>
    <ul>
      <li>Membuat portofolio yang menarik</li>
      <li>Mengedit menggunakan Canva</li>
      <li>Membuat prompt ChatGPT</li>
      <li>Keterampilan digital lainnya</li>
    </ul>
    <p>Saya terus mengembangkan diri dalam dunia digital dan teknologi. Dengan semangat belajar yang tinggi, saya percaya bahwa setiap keterampilan akan menjadi bekal berharga untuk masa depan saya.</p>
  </div>

  <script>
    function showPage(pageId) {
      // Sembunyikan semua halaman
      document.querySelectorAll('.page').forEach(function(page) {
        page.classList.remove('active');
      });

      // Tampilkan halaman yang dipilih
      document.getElementById(pageId).classList.add('active');
    }
  </script>

</body>
</html>
