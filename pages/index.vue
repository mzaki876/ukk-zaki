<template>
  <div class="news-page">
    <header class="news-header">
      <p>Selamat Datang di Website SMKN4 Tasikmalaya</p>
    </header>
    <section class="news-list">
      <div v-for="newsItem in news" :key="newsItem.id" class="news-card">
        <img :src="newsItem.image" :alt="newsItem.title" class="news-image" />
        <div class="news-content">
          <h2 class="news-title">{{ newsItem.title }}</h2>
          <p class="news-summary">{{ newsItem.summary }}</p>
        </div>
      </div>
    </section>
  </div>
  <!-- Pendidik dan Tenaga Kependidikan -->
  <div class="col-lg-12 mb-3">
    <div class="card">
      <div class="card-header bg-secondary text-white">
        <h5 class="text-center">Pendidik dan Tenaga Kependidikan</h5>
      </div>
      <div class="card-body">
        <div class="row">
          <!-- Jumlah Guru PNS -->
          <div class="col-md-6 mb-3">
            <div class="card">
              <div class="card-header bg-secondary text-white">
                <h6 class="text-center mb-0">Jumlah Guru PNS</h6>
              </div>
              <div class="card-body">
                <p>Laki-laki: 7 orang</p>
                <p>Perempuan: 3 orang</p>
                <p>Total: 10 orang</p>
              </div>
            </div>
          </div>
          <!-- Jumlah Guru Honorer -->
          <div class="col-md-6 mb-3">
            <div class="card">
              <div class="card-header bg-secondary text-white">
                <h6 class="text-center mb-0">Jumlah Guru Honorer</h6>
              </div>
              <div class="card-body">
                <p>Laki-laki: 20 orang</p>
                <p>Perempuan: 10 orang</p>
                <p>Total: 30 orang</p>
              </div>
            </div>
          </div>
          <!-- Jumlah Tenaga Administrasi PNS -->
          <div class="col-md-6 mb-3">
            <div class="card">
              <div class="card-header bg-secondary text-white">
                <h6 class="text-center mb-0">Jumlah Tenaga Administrasi PNS</h6>
              </div>
              <div class="card-body">
                <p>Laki-laki: 2 orang</p>
                <p>Perempuan: 1 orang</p>
                <p>Total: 3 orang</p>
              </div>
            </div>
          </div>
          <!-- Jumlah Tenaga Administrasi Honorer -->
          <div class="col-md-6 mb-3">
            <div class="card">
              <div class="card-header bg-secondary text-white">
                <h6 class="text-center mb-0">Jumlah Tenaga Administrasi Honorer</h6>
              </div>
              <div class="card-body">
                <p>Laki-laki: 3 orang</p>
                <p>Perempuan: 2 orang</p>
                <p>Total: 5 orang</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="content">
    <h2>Statistik Data</h2>
    <div class="stats-grid">
      <div class="stat-item">
        <h3>Jumlah Siswa</h3>
        <p class="value">1116</p>
      </div>
      <div class="stat-item">
        <h3>Jumlah Rombel</h3>
        <p class="value">34</p>
      </div>
      <div class="stat-item">
        <h3>Jumlah Guru</h3>
        <p class="value">60</p>
      </div>
      <div class="stat-item">
        <h3>Jumlah Tenaga Administrasi</h3>
        <p class="value">10</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  name: "BeritaPage",
  data() {
    return {
      news: [
        {
          id: 2,
          title: "MERAIH JUARA LKS RPL",
          summary: "Enam siswa SMKN4 meraih juara LKS RPL.",
          image: "https://radartasik.id/wp-content/uploads/2023/04/LKS-RPL.jpg",
        },
        {
          id: 3,
          title: "TUJUH SISWA SMKN4 MENDAPATKAN BEASISWA",
          summary: "Tujuh siswa smkn4 mendapatkan beasiswa dari Astra Honda Motor.",
          image: "https://assets.radartasik.id/main/2024/10/SMKN-4-tasikmalaya-raih-beasiswa-AHM.webp",
        },
        {
          id: 1,
          title: "PERESMIAN KERJA SAMA ",
          summary: "Peresmian kerja sama dengan Astra Hondra Motor.",
          image: "https://asset-2.tstatic.net/jabar/foto/bank/images/Peresmian-antara-PT-Daya-Adicipta-Motora-dan-SMK-Negeri-4-Tasikmalaya.jpg",
        },
      ],
    };
  },
};
</script>

<style>
.news-page {
  font-family: "Arial", sans-serif;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
  text-align: center;
}

/* Header */
.news-header {
  margin-bottom: 30px;;
}

.news-header h1 {
  font-size: 2.5rem;
  color: #333;
  margin-bottom: 10px;
}

.news-header p {
  font-size: 1.2rem;
  color: #666;
}

/* Daftar Berita */
.news-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  margin-top: 20px;
}

/* Kartu Berita */
.news-card {
  background-color: white;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.news-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
}

/* Gambar Berita */
.news-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

/* Konten Berita */
.news-content {
  padding: 15px;
}

.news-title {
  font-size: 1.5rem;
  color: #333;
  margin-bottom: 10px;
}

.news-summary {
  font-size: 1rem;
  color: #555;
  margin-bottom: 15px;
}



body {
  margin: 0;
  font-family: Arial, sans-serif;
  background-color: #f9f9f9;
}

.container {
  display: flex;
  gap: 20px;
  padding: 20px;
}

/* Slider */
.slider {
  flex: 3;
  position: relative;
  background-color: #fff;
  box-shadow: 0px 2px 5px rgba(0, 0, 0, 0.1);
  border-radius: 8px;
  overflow: hidden;
}

.slider-content {
  padding: 20px;
  text-align: center;
}

.slider-content h2 {
  font-size: 18px;
  background-color: rgba(0, 0, 0, 0.7);
  color: #fff;
  padding: 10px;
  border-radius: 5px;
}

.slider-content p {
  margin: 10px 0;
  font-size: 14px;
  color: #555;
}

.slider-image {
  width: 100%;
  height: auto;
  margin: 10px 0;
}

.slider-footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.btn-berita {
  background-color: #007bff;
  color: #fff;
  padding: 8px 15px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.btn-berita:hover {
  background-color: #0056b3;
}

.tanggal {
  font-size: 12px;
  color: #888;
}

.marquee-text {
  width: 100%;
  font-size: 14px;
  color: #555;
}
.card-header {
  font-weight: bold;
  font-size: 1.1rem;
}
.card-body p {
  margin-bottom: 10px;
  text-align: justify;
}

.stats-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
}

.stat-item {
  background-color:gray;
  padding: 20px;
  border-radius: 8px;
  text-align: center;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.stat-item h3 {
  margin-bottom: 10px;
}

.stat-item .value {
  font-size: 24px;
  font-weight: bold;
}
</style>
