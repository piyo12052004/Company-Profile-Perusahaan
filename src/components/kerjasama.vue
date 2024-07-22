<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <div>
        <div class="bekerjaSamaDengan">
            <p>Pernah Bekerjasama Dengan</p>
        </div>
        <div class="img-client">
            <div class="moving-images">
                <img v-for="(image, index) in images" :key="'client-' + index" :src="image" class="moving-image" />
                <img v-for="(image, index) in images" :key="'client-duplicate-' + index" :src="image"
                    class="moving-image" />
                <img v-for="(image, index) in images" :key="'client-duplicate-' + index" :src="image"
                    class="moving-image" />
            </div>
        </div>
        <div class="imgclientr">
            <div class="moving-images">
                <img v-for="(image, index) in images" :key="'clientr-' + index" :src="image" class="moving-image" />
                <img v-for="(image, index) in images" :key="'clientr-duplicate-' + index" :src="image"
                    class="moving-image" />
                <img v-for="(image, index) in images" :key="'clientr-duplicate-' + index" :src="image"
                    class="moving-image" />
            </div>
        </div>
    </div>
</template>

<script lang="ts" setup>
const images = [
    require('../assets/img/baiksan.png'),
    require('../assets/img/hilon.png'),
    require('../assets/img/hoa.png'),
    require('../assets/img/McDonalds.png'),
    require('../assets/img/Mitsui.png'),
    require('../assets/img/Nippon.png'),
    require('../assets/img/pngegg.png'),
    require('../assets/img/pngwing.png'),
    require('../assets/img/PT_Jui.png'),
    require('../assets/img/PT_Supreme.png'),
    require('../assets/img/pt-inocycle.png'),
    require('../assets/img/Shabu.png'),
    require('../assets/img/SOLAR.png'),
    require('../assets/img/SSA.png'),
    require('../assets/img/UNIQLO.png'),
    require('../assets/img/Vantec.png'),
    require('../assets/img/Yamaha.png'),
];
</script>

<style scoped>
.bekerjaSamaDengan {
    font-size: 28px;
    font-weight: bold;
    margin-bottom: 20px;
}

.img-client,
.imgclientr {
    display: flex;
    overflow: hidden;
    /* Agar gambar yang keluar dari container tidak terlihat */
    white-space: nowrap;
    /* Mencegah pembungkusan baris pada elemen flex */
}

.imgclientr {
    margin-top: 20px;
}

.img-client .moving-images,
.imgclientr .moving-images {
    display: flex;
}

.img-client .moving-images {
    animation: moveLeft 20s linear infinite;
}

.imgclientr .moving-images {
    animation: moveRight 20s linear infinite;
}

.moving-image {
    width: 200px;
    /* Sesuaikan dengan lebar yang diinginkan */
    height: 100px;
    /* Agar gambar tetap proporsional */
    padding-left: 10px;
}

@keyframes moveLeft {
    from {
        transform: translateX(0);
    }

    to {
        transform: translateX(-100%);
    }
}

@keyframes moveRight {
    from {
        transform: translateX(-100%);
    }

    to {
        transform: translateX(0);
    }
}

@media (max-width: 600px) {
    .moving-image {
    width: 100px;
    /* Sesuaikan dengan lebar yang diinginkan */
    height: 50px;
    /* Agar gambar tetap proporsional */
    padding-left: 10px;
}
.bekerjaSamaDengan {
    font-size: 20px;
    font-weight: bold;
    margin-bottom: 20px;
}
}
</style>