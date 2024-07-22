<template>
    <div class="destop">
        <div>
            <div class="navigasi">
                <ul>
                    <li><a translate="no" href="https://mail.google.com/mail/u/0/#inbox?compose=new" class="titleCore"><i
                                class="bi bi-envelope-at"></i> {{ email }}</a></li>
                    <li><a href="" class="titleCore"> <i class="bi bi-geo-alt-fill"></i> Grand Galaxy City, RSNB No. 22,
                            Bekasi</a></li>
                    <FeatherIcon icon="alert-circle" style="color: #000;" />
                </ul>
            </div>
            <div class="logoMain">
                <FeatherIcon icon="alert-circle" />
            </div>
        </div>
        <div class="logoWhatsAap">
            <div>
                <!-- <a :href="whatsappLink" target="_blank"> -->
                <a href="https://wa.me/6281285611255?text=Halo,%20Natanusa" target="_blank">
                    <svg xmlns="http://www.w3.org/2000/svg" color="#198754" width="56" height="56" fill="currentColor"
                        class="bi bi-whatsapp" viewBox="0 0 16 16">
                        <path
                            d="M13.601 2.326A7.85 7.85 0 0 0 7.994 0C3.627 0 .068 3.558.064 7.926c0 1.399.366 2.76 1.057 3.965L0 16l4.204-1.102a7.9 7.9 0 0 0 3.79.965h.004c4.368 0 7.926-3.558 7.93-7.93A7.9 7.9 0 0 0 13.6 2.326zM7.994 14.521a6.6 6.6 0 0 1-3.356-.92l-.24-.144-2.494.654.666-2.433-.156-.251a6.56 6.56 0 0 1-1.007-3.505c0-3.626 2.957-6.584 6.591-6.584a6.56 6.56 0 0 1 4.66 1.931 6.56 6.56 0 0 1 1.928 4.66c-.004 3.639-2.961 6.592-6.592 6.592m3.615-4.934c-.197-.099-1.17-.578-1.353-.646-.182-.065-.315-.099-.445.099-.133.197-.513.646-.627.775-.114.133-.232.148-.43.05-.197-.1-.836-.308-1.592-.985-.59-.525-.985-1.175-1.103-1.372-.114-.198-.011-.304.088-.403.087-.088.197-.232.296-.346.1-.114.133-.198.198-.33.065-.134.034-.248-.015-.347-.05-.099-.445-1.076-.612-1.47-.16-.389-.323-.335-.445-.34-.114-.007-.247-.007-.38-.007a.73.73 0 0 0-.529.247c-.182.198-.691.677-.691 1.654s.71 1.916.81 2.049c.098.133 1.394 2.132 3.383 2.992.47.205.84.326 1.129.418.475.152.904.129 1.246.08.38-.058 1.171-.48 1.338-.943.164-.464.164-.86.114-.943-.049-.084-.182-.133-.38-.232" />
                    </svg>
                </a>
            </div>
        </div>
    </div>
</template>
<script lang="ts" setup>
// const phoneNumber = '6281285611255 '; // Ganti dengan nomor telepon tujuan
// const message = 'Halo, saya tertarik dengan produk Anda.'; // Ganti dengan pesan yang ingin dikirim
// const whatsappLink = `https://wa.me/${phoneNumber}?text=${encodeURIComponent(message)}`;
// const whatsappLink = `https://wa.me/${phoneNumber}`;
const email = 'hello@natanusaayudhri.com';
</script>

<style scoped>
.navigasi {
    background-color: #3687aa;
    width: 100%;
    height: 50px;
    display: flex;
    list-style-type: none;
    justify-content: end;
    align-items: center;
    text-align: center;
}

.titleCore {
    color: white;
    text-decoration: none;
}

.navigasi ul {
    display: flex;
    list-style-type: none;
    justify-content: end;
    align-items: center;
    text-align: center;
}

.navigasi ul li {
    margin-right: 20px;
}
.logoWhatsAap{
    position: fixed;
    right: 50px;
    top: 450px;    
    z-index: 100;
}
@media (max-width: 600px) {
    .destop {
        display: none;
    }
}

</style>
