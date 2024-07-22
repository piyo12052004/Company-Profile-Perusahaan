<template>
    <div>
        <div class="destop">
            <div class="mainnArtikel">
                <div class="titleMain">
                    <p class="artikeltitle1">Articles and News</p>
                    <p>Articles are written based on experience and portfolio while in the field</p>
                </div>
                <div class="viewTampilan">
                    <div class="blog  rounded-lg shadow">
                        <a href="artikel">
                            <h5 class="mb-2 text-2xl font-bold tracking-tight  dark:text-white text-white">The Importance of SLF for Factory Buildings</h5>
                        </a>
                        <p class="mb-3 font-normal text-white dark:text-gray-400">MAR 15</p>
                        <a href="artikel"
                            class="inline-flex items-center px-3 py-2 mt-56 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
                            style="bottom: 0px;">
                            Read more
                            <svg class="rtl:rotate-180 w-3.5 h-3.5 ms-2" aria-hidden="true"
                                xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 10">
                                <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                    stroke-width="2" d="M1 5h12m0 0L9 1m4 4L9 9" />
                            </svg>
                        </a>
                    </div>

                </div>
            </div>
        </div>
        <div class="AppMobilee">
            <div class="mainnn">
                <div class="titleMain">
                    <p class="artikeltitle1">Articles and News</p>
                    <p style="font-size: 12px; " class="px-5">Articles are written based on experience and portfolio while in the field</p>
                </div>
                <div class="viewTampilan">
                    <div class="blog  rounded-lg shadow">
                        <router-link to="/artikel">
                            <h5 class="mb-2 text-2xl font-bold tracking-tight  dark:text-white text-white">The Importance of SLF for Factory Buildings</h5>
                        </router-link>
                        <p class="mb-3 font-normal text-white dark:text-gray-400">MAR 15</p>
                         <router-link to="/artikel"
                            class="inline-flex items-center px-3 py-2 mt-32 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
                            style="bottom: 0px;">
                            Read more
                            <svg class="rtl:rotate-180 w-3.5 h-3.5 ms-2" aria-hidden="true"
                                xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 10">
                                <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                                    stroke-width="2" d="M1 5h12m0 0L9 1m4 4L9 9" />
                            </svg>
                        </router-link>
                    </div>

                </div>
            </div>
        </div>
    </div>
</template>

<script>
</script>

<style>
@media (min-width: 1280px) {
.AppMobilee{
    display: none;
}
.main {
    padding-top: 50px;
}

.artikeltitle1 {
    font-weight: bold;
    font-size: 38px;
}

.blog {
    background: url('../assets/img/img1.jpg');
    width: 300px;
    height: 400px;
    position: relative;
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    color: #fff;
    text-align: left;
    padding: 10px;
    margin: 20px;
}
}
@media (max-width: 600px) {
    .destop{
        display: none;
    }
   .mainn {
    padding-top: 50px;
}
/* .AppMobilee{
    margin-top: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
} */

.artikeltitle1 {
    font-weight: bold;
    font-size: 20px;
}

.blog {
    background: url('../assets/img/img1.jpg');
    width: 280px;
    height: 300px;
    position: relative;
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    color: #fff;
    text-align: left;
    padding: 10px;
    margin: 20px;
}
.mainnArtikel{
    margin-top: 20px;
}
}
</style>