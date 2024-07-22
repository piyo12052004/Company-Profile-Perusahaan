<template>
  <div class="container">
    <section>
      <headNav/>
    </section>
    <div class="home">
      <section class="views1">
        <dashboardlayouts />
      </section>
      <div class="isi">
        <section class="section2" id="tentangSaya">
          <tentangPerusahanVuee />
        </section>
      </div>
      <section class="section5" id="Kerjasama"> 
        <Kerjasama/>
      </section>
      <section class="section3" id="konsultasi"> 
        <formEmail/>
      </section>
      <section class="section4" id="artikel">
        <artikelDanBeritaVue/>
      </section>
      <section class="footer">
        <footerr/>
      </section>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import tentangPerusahanVuee from '@/components/tentangPerusahan.vue'
import dashboardlayouts from '@/components/dashboardlayouts.vue';
import formEmail from '@/components/formEmail.vue';
import footerr from '@/components/footer.vue';
import artikelDanBeritaVue from '@/components/artikelDanBerita.vue';
import headNav from '@/components/headerNav.vue'
import Kerjasama from '@/components/kerjasama.vue'

export default {
  name: 'HomeView',
  components: {
    tentangPerusahanVuee,
    dashboardlayouts,
    formEmail,
    footerr,
    artikelDanBeritaVue,
    headNav,
    Kerjasama
  },
  views: {
  }
}
</script>

<style>
.container {
  margin-left: auto;
  margin-right: auto;
}

.isi {
  margin-left: 1%;
  margin-right: 1%;
}
.section2{
  padding-top: 100px;
  padding-bottom: 100px;
}

.views1 {
  position: relative;
  width: 100%;
  height: 500px;
  /* Sesuaikan sesuai kebutuhan Anda */
  background-image: url('../assets/img/bagroundImage.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  color: #fff;
  /* Warna teks agar kontras dengan gambar */
  /* display: flex;
      justify-content: center;
      align-items: center;
      text-align: center; */
}

.views1::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(255, 255, 255, 0.5);
  /* Overlay putih dengan opacity 0.5 */
  /* Atau bisa menggunakan warna lain, seperti rgba(0, 0, 0, 0.5) untuk hitam */
  pointer-events: none;
  /* Agar overlay tidak mengganggu interaksi dengan konten di atasnya */
}

.views1>* {
  position: relative;
  /* Memastikan konten berada di atas overlay */
}
.section3{
  position: relative;
  width: 100%;
  /* height: 500px; */
  /* Sesuaikan sesuai kebutuhan Anda */
  background-image: url('../assets/img/images.png');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  
  color: #fff;
}
.section3::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(255, 255, 255, 0.5);
  /* Overlay putih dengan opacity 0.5 */
  /* Atau bisa menggunakan warna lain, seperti rgba(0, 0, 0, 0.5) untuk hitam */
  pointer-events: none;
  /* Agar overlay tidak mengganggu interaksi dengan konten di atasnya */
}

.section3>* {
  position: relative;
  /* Memastikan konten berada di atas overlay */
}
.section5{
  /* margin-top: 100px; */
  margin-bottom: 100px;
}
@media (max-width: 600px) {
  .section2{
    padding-top: 30px;
    padding-bottom: 30px;
  }
  .section4{
    padding-top: 30px;
  }

}
</style>
