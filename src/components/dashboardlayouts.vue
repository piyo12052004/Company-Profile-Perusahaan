<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <div class="maintextview1"
        data-aos="fade-right"
       data-aos-duration="1000"
        data-aos-easing="ease-in-sine"
    >
        <div class="isitext">
            <div class="text1">
                <p>Trusted SLF Consultant</p>
            </div>
            <div class="text2">
                <p>Looking for professional SLF technical assessors and consultants?</p>
            </div>
            <div class="text3">
                <p>PT Natanusa Wahana Bahtera is the right solution to be a partner in taking care of all building permits, both PBG, SLF, environmental permits, K3 recommendations, and others</p>
            </div>
            <div style="margin-top: 20px;">
                <a href="https://wa.me/6281285611255?text=Halo,%20Natanusa" class="focus:outline-none text-white bg-green-700 hover:bg-green-800 focus:ring-4 focus:ring-green-300 font-medium rounded-lg text-sm px-5 py-2.5 me-2 mb-2 dark:bg-green-600 dark:hover:bg-green-700 dark:focus:ring-green-800">WhatsApp 
                    <i class="bi bi-whatsapp"></i>
                </a>
            </div>
        </div>
    </div>
</template>

<style>
.text3 p {
    font-size: 15px;
}
.text1 p{
    font-size: 22px;
    font-weight: bold;
    color: #3687aa;
}
.text2{
    font-weight: bold;
    font-size: 30px;
}
.maintextview1 {
    text-align: left;
    display: flex;
    height: 500px;
    justify-content: left;
    align-items: center;
}
.isitext{
    /* position: absolute; */
    width: 500px;
    margin-left: 50px;
}
p{
    color: black;
}

@media (max-width: 600px) {
    .maintextview1{
        text-align: left;
        display: flex;
        height: 500px;
        justify-content: left;
        
    }
    .isitext{
        margin-left: 10px;
    }
    .text2{
        font-size: 20px;
    }
    .text1 p{
        font-size: 15px;
    }
    .text3 p{
        font-size: 12px;
    }
}

</style>
