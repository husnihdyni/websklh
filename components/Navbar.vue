<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container">
        <a class="navbar-brand d-flex align-items-center" href="#">
          <img src="/assets/img/smkn4.jpg" alt="Logo" width="30" height="30" class="me-2">
          SMK NEGERI 4 TASIKMALAYA
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <nuxt-link to="/" class="nav-link" aria-current="page">Home</nuxt-link>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="ProfileDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">Profile</a>
              <ul class="dropdown-menu" aria-labelledby="ProfileDropdown">
                <li><nuxt-link to="/Profile/identitas" class="dropdown-item">Identitas</nuxt-link></li>
                <li><nuxt-link to="/Profile/jurusan" class="dropdown-item">Jurusan</nuxt-link></li>
                <li><nuxt-link to="/Profile/sejarah" class="dropdown-item">Sejarah</nuxt-link></li>
                <li><nuxt-link to="/Profile/visi-misi" class="dropdown-item">Visi-Misi</nuxt-link></li>
              </ul>
            </li>
            <li class="nav-item">
                <li><nuxt-link to="/Ekstrakurikuler/eskul" class="dropdown-item">Ekstrakulikuler</nuxt-link></li>
            </li>
            <li class="nav-item">
              <nuxt-link to="/galeri/foto-foto" class="nav-link">Galeri</nuxt-link>
            </li>
            <li class="nav-item">
              <nuxt-link to="/berita/informasi" class="nav-link">Berita</nuxt-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <div class="container mt-4">
      <NuxtPage />
    </div>
  </div>
</template>

<script setup>
</script>


