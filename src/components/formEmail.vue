<template>
    <div>
        <div class="">
            <div class="main">
                <div class="CoreFrom">
                    <div class="titleFrom">
                        <p class="title1" data-aos="fade-up" data-aos-duration="1000">Get best price from Natanusa
                        </p>
                        <p class="title2" data-aos="fade-up" data-aos-duration="1000">
                            We will provide the best price quote (our version) for you. Please tell us your company's needs through the following message box.
                        </p>
                        <div class="listtittelform">
                            <ul class="space-y-4 text-gray-500 list-disc list-inside dark:text-gray-400">
                                <li class="" data-aos="fade-up" data-aos-duration="1000">
                                    <span class="titlelist">Identify client needs</span>
                                    <ol class="ps-5 mt-2 space-y-1 list-inside">
                                        <li>
                                            <p>We will look at and analyze your needs before proceeding to the process of creating a quote</p>
                                        </li>
                                    </ol>
                                </li>
                                <li data-aos="fade-up" data-aos-duration="1000">
                                    <span class="titlelist"> Bid creation</span>
                                    <ul class="ps-5 mt-2 space-y-1 list-inside">
                                        <li>
                                            <p>We will send you a quote for the job by email</p>
                                        </li>
                                    </ul>
                                </li>
                                <li data-aos="fade-up" data-aos-duration="1000">
                                    <span class="titlelist">Contracts and cooperation</span>
                                    <ul class="ps-5 mt-2 space-y-1 list-inside">
                                        <li>
                                            In order to establish a professional partnership, we will make an employment contract in accordance with the applicable laws in Indonesia
                                        </li>
                                    </ul>
                                </li>
                                <li data-aos="fade-up" data-aos-duration="1000">
                                    <span class="titlelist">Work begins</span>
                                    <ul class="ps-5 mt-2 space-y-1 list-inside">
                                        <li>
                                            <p>
                                                During the work, there will be a monitoring and evaluation process that is carried out periodically to ensure quality and timeliness
                                            </p>
                                        </li>
                                    </ul>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="titleFrom2">
                        <form class="max-w-md mx-auto" action="post" ref="form" method="" @submit.prevent="sendEmail">
                            <h2 class="text-black font-bold text-2xl">Free and Fast Consultation</h2>
                            <div class="relative z-0 w-full mb-5 group">
                                <input type="text" name="floating_namaLengkap" id="floating_namaLengkap"
                                    class="  block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-600 dark:focus:border-blue-500 focus:outline-none focus:ring-0 focus:border-blue-600 peer"
                                    placeholder=" " required />
                                <label for="floating_namaLengkap"
                                    class="inputMobile peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:start-0 rtl:peer-focus:translate-x-1/4 rtl:peer-focus:left-auto peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">Full name</label>
                            </div>
                            <div class="relative z-0 w-full mb-5 group">
                                <input type="email" name="floating_email" id="floating_email"
                                    class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-600 dark:focus:border-blue-500 focus:outline-none focus:ring-0 focus:border-blue-600 peer"
                                    placeholder=" " required />
                                <label for="floating_email"
                                    class="inputMobile peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:start-0 rtl:peer-focus:translate-x-1/4 peer-focus:left-auto peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">Active email</label>
                            </div>
                            <div class="relative z-0 w-full mb-5 group">
                                <input type="text" name="floating_Hal" id="floating_Hal"
                                    class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-600 dark:focus:border-blue-500 focus:outline-none focus:ring-0 focus:border-blue-600 peer"
                                    placeholder=" " required />
                                <label for="floating_Hal"
                                    class="inputMobile peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:start-0 rtl:peer-focus:translate-x-1/4 peer-focus:left-auto peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">Hal (subject)</label>
                            </div>
                            <div class="relative z-0 w-full mb-5 group">
                                <input type="text" name="floating_pesanAnda" id="floating_pesanAnda"
                                    class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-600 dark:focus:border-blue-500 focus:outline-none focus:ring-0 focus:border-blue-600 peer"
                                    placeholder=" " required />
                                <label for="floating_pesanAnda"
                                    class="inputMobile peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:start-0 rtl:peer-focus:translate-x-1/4 peer-focus:left-auto peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">Your Message</label>
                            </div>
                            <button type="submit"
                                class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm w-full sm:w-auto px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                                Submit
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
        <!-- <div class="appmobile">
            <div class="titleFrom2">
                <form class="max-w-md mx-auto" action="post" ref="form" method="" @submit.prevent="sendEmail">
                    <h2 class="text-black font-bold text-lg flex pb-5">Konsultasi Gratis dan Cepat</h2>
                    <div class="relative z-0 w-full mb-5 group">
                        <input type="text" name="floating_namaLengkap" id="floating_namaLengkap"
                            class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-600 dark:focus:border-blue-500 focus:outline-none focus:ring-0 focus:border-blue-600 peer"
                            placeholder=" " required />
                        <label for="floating_namaLengkap"
                            class="text-left flex peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:start-0 rtl:peer-focus:translate-x-1/4 rtl:peer-focus:left-auto peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">Nama
                            Lengkap</label>
                    </div>
                    <div class="relative z-0 w-full mb-5 group">
                        <input type="email" name="floating_email" id="floating_email"
                            class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-600 dark:focus:border-blue-500 focus:outline-none focus:ring-0 focus:border-blue-600 peer"
                            placeholder=" " required />
                        <label for="floating_email"
                            class=" text-left flex peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:start-0 rtl:peer-focus:translate-x-1/4 peer-focus:left-auto peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">Email
                            Aktif</label>
                    </div>
                    <div class="relative z-0 w-full mb-5 group">
                        <input type="text" name="floating_Hal" id="floating_Hal"
                            class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-600 dark:focus:border-blue-500 focus:outline-none focus:ring-0 focus:border-blue-600 peer"
                            placeholder=" " required />
                        <label for="floating_Hal"
                            class="text-left flex peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:start-0 rtl:peer-focus:translate-x-1/4 peer-focus:left-auto peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">Hal
                            (subject)</label>
                    </div>
                    <div class="relative z-0 w-full mb-5 group">
                        <input type="text" name="floating_pesanAnda" id="floating_pesanAnda"
                            class="block py-2.5 px-0 w-full text-sm text-gray-900 bg-transparent border-0 border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-600 dark:focus:border-blue-500 focus:outline-none focus:ring-0 focus:border-blue-600 peer"
                            placeholder=" " required />
                        <label for="floating_pesanAnda"
                            class="text-left flex peer-focus:font-medium absolute text-sm text-gray-500 dark:text-gray-400 duration-300 transform -translate-y-6 scale-75 top-3 -z-10 origin-[0] peer-focus:start-0 rtl:peer-focus:translate-x-1/4 peer-focus:left-auto peer-focus:text-blue-600 peer-focus:dark:text-blue-500 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-6">Pesan
                            Anda</label>
                    </div>
                    <button type="submit"
                        class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm w-full sm:w-auto px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                        Submit
                    </button>
                </form>
            </div>
        </div> -->
    </div>

</template>

<script>
import emailjs from '@emailjs/browser';
import Swal from 'sweetalert2';

export default {
    methods: {
        sendEmail() {
            emailjs
                .sendForm('service_pq2b5cu', 'template_mehgxaz', this.$refs.form, '6Ku88s0C_SrUgKZPg')
                .then(
                    () => {
                        Swal.fire({
                            icon: 'success',
                            title: 'Berhasil!',
                            text: 'Pesan Anda telah terkirim.',
                            confirmButtonText: 'OK',
                        });
                    },
                    (error) => {
                        Swal.fire({
                            icon: 'error',
                            title: 'Gagal!',
                            text: 'Terjadi kesalahan saat mengirim pesan: ' + error.text,
                            confirmButtonText: 'OK',
                        });
                    },
                );
        },
    },
};
</script>

<style>
@media (min-width: 1280px) {
    .appmobile {
        display: none;
    }

    .titleFrom,
    .titleFrom2 {
        text-align: left;
    }

    .CoreFrom {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        gap: 22px;
        padding-top: 50px;
        padding-bottom: 50px;
        width: 1000px;
    }

    .title1 {
        font-size: 38px;
        font-weight: bold;
    }

    .titleFrom {
        padding-left: 50px;
        padding-right: 50px;
    }

    .main {
        display: flex;
        justify-content: center;
    }

    .listtittelform {
        color: black;
        padding-top: 20px;
    }

    .titlelist {
        color: black;
        font-weight: bold;
        font-size: 18px;
    }
}

@media (max-width: 600px) {
    .destop {
        display: none;
    }

    .titleFrom2 {
        margin-left: 10px;
        margin-right: 10px;
    }
    .titleFrom{
        display: none;
    }
    .inputMobile{
        text-align: left;
        display: flex;
    }
}
</style>