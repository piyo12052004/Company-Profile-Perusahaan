<template>
  <div class="pembatasheader">
    <div class="destop">
      <div>
        <nav :class="['nav', { 'navbar-visible': isVisible, }]">
          <div class="logo">
            <img src="../assets/img/LogoHead.png" alt="Logo">
          </div>
          <div class="search">
            <ul>
              <li><a href="#">Home</a></li>
              <li><a href="#tentangSaya">About Me</a></li>
              <li><a href="#konsultasi">Consultant</a></li>
              <li><a href="#kerjasama">Have Worked Together</a></li>
              <li><a href="#artikel">Article</a></li>
            </ul>
          </div>
        </nav>
        <!-- Konten halaman lainnya -->
      </div>
    </div>
    <!-- drawer init and toggle -->
    <div class="drawerMenu  text-center">
      <div class="logo">
        <img src="../assets/img/LogoHead.png" alt="Logo">
      </div>
      <!-- <button
        class="text-black  focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm dark:bg-blue-600 dark:hover:bg-blue-700 focus:outline-none dark:focus:ring-blue-800"
        type="button" data-drawer-target="dropdownHover" data-drawer-show="dropdownHover" data-drawer-placement="right"
        aria-controls="dropdownHover">
        <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" fill="currentColor" class="bi bi-list"
          viewBox="0 0 16 16">
          <path fill-rule="evenodd"
            d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5" />
        </svg>
      </button> -->
      <button id="dropdownHoverButton" data-dropdown-toggle="dropdownHover" data-dropdown-trigger="hover"
        class="text-white focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center inline-flex items-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
        type="button"><svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" fill="currentColor" class="bi bi-list"
          viewBox="0 0 16 16">
          <path fill-rule="evenodd"
            d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5m0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5" />
        </svg>
      </button>

      <div class="logoWhatsAap">
            <div>
                <!-- <a :href="whatsappLink" target="_blank"> -->
                <a href="https://wa.me/6281285611255?text=Halo,%20Natanusa" target="_blank">
                    <svg xmlns="http://www.w3.org/2000/svg" color="#198754" width="46" height="46" fill="currentColor"
                        class="bi bi-whatsapp" viewBox="0 0 16 16">
                        <path
                            d="M13.601 2.326A7.85 7.85 0 0 0 7.994 0C3.627 0 .068 3.558.064 7.926c0 1.399.366 2.76 1.057 3.965L0 16l4.204-1.102a7.9 7.9 0 0 0 3.79.965h.004c4.368 0 7.926-3.558 7.93-7.93A7.9 7.9 0 0 0 13.6 2.326zM7.994 14.521a6.6 6.6 0 0 1-3.356-.92l-.24-.144-2.494.654.666-2.433-.156-.251a6.56 6.56 0 0 1-1.007-3.505c0-3.626 2.957-6.584 6.591-6.584a6.56 6.56 0 0 1 4.66 1.931 6.56 6.56 0 0 1 1.928 4.66c-.004 3.639-2.961 6.592-6.592 6.592m3.615-4.934c-.197-.099-1.17-.578-1.353-.646-.182-.065-.315-.099-.445.099-.133.197-.513.646-.627.775-.114.133-.232.148-.43.05-.197-.1-.836-.308-1.592-.985-.59-.525-.985-1.175-1.103-1.372-.114-.198-.011-.304.088-.403.087-.088.197-.232.296-.346.1-.114.133-.198.198-.33.065-.134.034-.248-.015-.347-.05-.099-.445-1.076-.612-1.47-.16-.389-.323-.335-.445-.34-.114-.007-.247-.007-.38-.007a.73.73 0 0 0-.529.247c-.182.198-.691.677-.691 1.654s.71 1.916.81 2.049c.098.133 1.394 2.132 3.383 2.992.47.205.84.326 1.129.418.475.152.904.129 1.246.08.38-.058 1.171-.48 1.338-.943.164-.464.164-.86.114-.943-.049-.084-.182-.133-.38-.232" />
                    </svg>
                </a>
            </div>
        </div>
    </div>

    <!-- drawer component -->
    <div id="dropdownHover"
      class="z-10 hidden text-center bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700">
      <ul class="py-2 text-sm text-gray-700 dark:text-gray-200" aria-labelledby="dropdownHoverButton">
        <li>
          <a href="#"
            class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Home</a>
        </li>
        <li>
          <a href="#tentangSaya"
            class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">About Me</a>
        </li>
        <li>
          <a href="#konsultasi"
            class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Consultant</a>
        </li>
        <li>
          <a href="#Kerjasama"
            class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Have Worked Together</a>
        </li>
        <li>
          <a href="#artikel" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Article</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref, onMounted, onUnmounted } from 'vue';

const isVisible = ref(false);

const handleScroll = () => {
  if (window.scrollY > 100) {
    isVisible.value = true;
  } else {
    isVisible.value = false;
  }
};

onMounted(() => {
  window.addEventListener('scroll', handleScroll);
});

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll);
});
</script>

<style scoped>
.drawerMenu {
  display: none;
}

.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-left: 20px;
  padding-right: 20px;
  position: fixed;
  top: 50px;
  left: 0;
  right: 0;
  transition: top 0.5s ease-in-out;
  background-color: white;
  border-bottom: 2px solid rgba(250, 0, 0, 0.55);
  /* Tambahkan background-color jika diperlukan */
  z-index: 1;
  /* Agar navigasi tetap di atas konten lainnya */
}

.navbar-visible {
  top: 0;
}

.logo img {
  width: 130px;
  height: 80px;
}

.search {
  width: 400px;
}

.search ul {
  display: flex;
  justify-content: space-between;
}

.search ul li a {
  font-weight: bold;
  position: relative;
  text-decoration: none;
  color: inherit;
}

.search ul li a:before {
  content: "";
  position: absolute;
  width: 0;
  height: 2px;
  bottom: -3px;
  left: 0;
  background-color: #3687aa;
  visibility: hidden;
  transition: all 0.5s ease-in-out;
}

.search ul li a:hover:before,
.search ul li a:focus:before {
  visibility: visible;
  width: 100%;
}

.search ul li a:hover,
.search ul li a:focus {
  color: #3687aa;
}

.cliksearch {
  padding: 10px;
}

.cliksearch i {
  font-size: 25px;
}

@media (max-width: 600px) {
  .destop {
    display: none;
  }

  .pembatasheader {
    background-color: #3687aa;
    text-align: end;
    display: flex;
    justify-content: end;

  }

  .drawerMenu {
    position: fixed;
    z-index: 100;
    background-color: rgba(0, 0, 0, 0.2);
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    padding-right: 10px;
  }

  .logo img {
    width: 70px;
    padding-left: 10px;
    height: 40px;
  }
  .logoWhatsAap{
    position: fixed;
    right: 25px;
    top: 600px;    
    z-index: 100;
}
}
</style>