<template>
    <div class="container-fluid">
        <div class="col-lg-12">
            <h5 class="text-white text-center rounded-3 p-2 m-3">
                GURU <b>SMKN 4 TASIKMALAYA</b>
            </h5>
        </div>
        <section class="gallery">
            <div class="galeri-item">
                <img src="/assets/img/guru1.jpg" alt="guru" class="galeri-image" />
                <p class="gallery-caption">Taufik Hidayat</p>
            </div>
            <div class="galeri-item">
                <img src="/assets/img/guru2.jpg" alt="guru" class="galeri-image" />
                <p class="gallery-caption">Zul Hilmi</p>
            </div>
            <div class="galeri-item">
                <img src="/assets/img/guru3.jpg" alt="guru" class="galeri-image" />
                <p class="gallery-caption">Lisye Diana</p>
            </div>
            <div class="galeri-item">
                <img src="/assets/img/guru4.jpg" alt="guru" class="galeri-image" />
                <p class="gallery-caption">Suminar</p>
            </div>
            <div class="galeri-item">
                <img src="/assets/img/guru5.jpg" alt="guru" class="galeri-image" />
                <p class="gallery-caption"></p>
            </div>
        </section>
    </div>
</template>

<style scoped>
.gallery {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
    margin: 20px 0;
}

.galeri-item {
    flex: 0 1 calc(20% - 20px); /* 5 items per row, minus gap */
    background-color: #f9f9f9;
    border: 1px solid #ddd;
    border-radius: 8px;
    padding: 10px;
    transition: transform 0.3s;
    text-align: center;
}

.galeri-item:hover {
    transform: scale(1.05);
}

.galeri-image {
    width: 100%; /* Ensures images take up the full container width */
    height: auto; /* Maintain aspect ratio */
    border-radius: 8px;
}

.galeri-caption {
    color: #000; /* Black text for better visibility */
    margin-top: 10px;
    font-size: 14px;
    font-weight: bold;
}

h5 {
    background-color: transparent; /* Removed black background */
    color: #000; /* Ensured text is still visible */
    font-weight: bold;
}
</style>
