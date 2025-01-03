<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-lg-12">
        <h5 style="background-color: white;" class="text-white text-center rounded-3 p-2 m-3">
          Ekstrakurikuler <b>SMKN 4 TASIKMALAYA</b>
        </h5>
      </div>
      <section class="galeri">
        <div class="galeri-item" v-for="(item, index) in eskulitem" :key="index">
          <img :src="item.img" :alt="item.caption" class="galeri-img" />
          <p class="galeri-caption">{{ item.caption }}</p>
        </div>
      </section>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      galeriItems: [
        { img: "/assets/img/voli1.jpg", caption: "Voli" },
        { img: "/assets/img/pmr1.png", caption: "PMR" },
        { img: "/assets/img/futsal.jpg", caption: "Futsal" },
        { img: "/assets/img/paskibra.png", caption: "Paskibra" },
        { img: "/assets/img/pd.png", caption: "Perisai Diri" },
        { img: "/assets/img/badminton.png", caption: "Badminton" },
        { img: "/assets/img/basket.jpg", caption: "Basket" },
      ],
    };
  },
};
</script>
<style scoped>
.galeri {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 20px;
  margin: 20px 0;
  padding: 0 10px;
}

.galeri-item {
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 10px;
  text-align: center;
  transition: transform 0.3s;
}

.galeri-item:hover {
  transform: scale(1.05);
}

.galeri-img {
  width: 100%;
  height: 150px;
  object-fit: cover;
  border-radius: 8px;
}

.galeri-caption {
  color: #333;
  margin-top: 10px;
  font-size: 1rem;
}
</style>


