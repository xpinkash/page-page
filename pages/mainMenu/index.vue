<template>
    <div class="main_content">
         <navi />
         <p><img src="~/assets/img/common/img01.png" alt=""></p>
         <div class="options">
            <h3>Options for Service</h3>
            <div class="services">
                <ul class="svr01">
                    <li><nuxt-link to="/washingmachine/"><img src="~/assets/img/common/img_01_service.png" alt=""></nuxt-link></li>
                    <li><nuxt-link to="/ref/"><img src="~/assets/img/common/img_02_service.png" alt=""></nuxt-link></li>
                    <li><nuxt-link to="/aircon/"><img src="~/assets/img/common/img_03_service.png" alt=""></nuxt-link></li>
                    <li><nuxt-link to="/vacuum/"><img src="~/assets/img/common/img_04_service.png" alt=""></nuxt-link></li>
                    <li><nuxt-link to="/ricecooker/"><img src="~/assets/img/common/img_05_service.png" alt=""></nuxt-link></li>
                    <li><nuxt-link to="/other/"><img src="~/assets/img/common/img_06_service.png" alt=""></nuxt-link></li>
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
    },
    
    data(){
        return{
            items: [
                { id:1, content: 'dsdsdsdsd'},
                { id:2, content: 'aaaaaaaaaaaaa'}
                ]
        }
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
    /* .page-enter-active {
      animation: acrossIn .20s ease-in ;
    } 
    .page-leave-active {
      animation: acrossOut .20s ease-out ;
    } 
    @keyframes acrossIn {
      0% {
        transform: translate3d(100%, 0, 0);
      }
      100% {
        transform: translate3d(0, 0, 0);
      }
    }
    @keyframes acrossOut {
      100% {
        transform: translate3d(100%, 0, 0);
      }
      0% {
        transform: translate3d(-0%, 0, 0);
      }
    } */
</style>
