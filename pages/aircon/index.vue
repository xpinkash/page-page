<template>
    <div class="main_content">
         <navi />
         <p><img src="~/assets/img/common/img01.png" alt=""></p>
         <div class="options">
            <h3>Aircon</h3>
            <div class="services">
                <ul class="svr01">
                    <li><nuxt-link to="/washingmachine/"><img src="~/assets/img/common/img_01_service.png" alt=""></nuxt-link></li>
                    <li><nuxt-link to="/ref/"><img src="~/assets/img/common/img_02_service.png" alt=""></nuxt-link></li>
                    <li><nuxt-link to="/aircon/"><img src="~/assets/img/common/img_03_service.png" alt=""></nuxt-link></li>
                </ul>
            </div>
         </div>
         <footerComponents />
    </div>
</template>

<script>
import navi from '@/components/headerComponents/navi'
import footerComponents from '@/components/footer/footerComponents'
export default {
    components: {
        navi,
        footerComponents
    }
}
</script>

<style scoped>

    p {
        line-height: 0;
        font-family: meiryo;
    }
    img {
        width: 100%;
    }
    .options {
        background: #d4d3ca;
        padding: 20px;
    }
    .svr01 {
        overflow: hidden;
        padding: 0;
    }
    .svr01 li {
        float: left;
        width: 49%;
        list-style-type: none;
    }
    .svr01 li:nth-child(2n+1){
        margin-right: 2%;
    }
    .services {
        margin: 15px 0;
    }
</style>
