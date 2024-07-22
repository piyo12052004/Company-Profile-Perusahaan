<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <div class="footer">
        <p>PT Natanusa WB © 2024. All rights reserved | <a href="https://mail.google.com/mail/u/0/#inbox?compose=new" translate="no" class="titleCore"> <i
            class="bi bi-envelope-at"></i> {{ email }}</a>| <i class="bi bi-whatsapp"></i> <a  href="https://wa.me/6281285611255?text=Halo,%20Natanusa">+62 812-8561-1255</a>  </p>
        
    </div>
</template>

<script lang="ts" setup>
const email = 'hello@natanusaayudhri.com';
</script>

<style>
.footer{
    background-color: #3687AA;
}
.footer p{
    padding: 20px;
}
@media (max-width: 600px) {
    .footer p{
    padding: 12px;
    font-size: 12px;
}
}

</style>