<template>
    <div class="main_content">
         <navi />
         <p><img src="~/assets/img/common/img01.png" alt=""></p>
         <div class="options">
            <h3>Washing Machine</h3>
            <div class="services">
                <!-- <ul>
                    <li v-for="(item, index) in items" :key="item.id" >
                        <p class="question">{{index+1}}. {{item.question}}</p>
                        <p class="content">Answer: <i>{{item.content}}</i></p>
                    </li>
                </ul> -->
                <ul class="svr01">
                    <li><nuxt-link to="/washingmachine/"><img src="~/assets/img/common/img_01_service.png" alt=""></nuxt-link></li>
                    <li><nuxt-link to="/ref/"><img src="~/assets/img/common/img_02_service.png" alt=""></nuxt-link></li>
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
                { id:1, question:'Lorem ipsum dolor sit amet, consectetur?' ,content: 'Washing Machine01'},
                { id:2, question:'Lorem ipsum dolor sit amet, consectetur?', content: 'Washing Machine01'},
                { id:3, question:'Lorem ipsum dolor sit amet, consectetur?', content: 'Washing Machine01'},
                { id:4, question:'Lorem ipsum dolor sit amet, consectetur?', content: 'Washing Machine01'},
                { id:5, question:'Lorem ipsum dolor sit amet, consectetur?', content: 'Washing Machine01'},
                { id:6, question:'Lorem ipsum dolor sit amet, consectetur?', content: 'Washing Machine01'},
                { id:7, question:'Lorem ipsum dolor sit amet, consectetur?', content: 'Washing Machine01'},
                ]
        }
    }
}
</script>

<style scoped>

    p {
        font-family: meiryo;
    }
    img {
        width: 100%;
        display: block;
    }
    .options {
        background: #d4d3ca;
        padding: 20px;
    }
    .services {
        margin: 15px 0;
    }
    .services ul li {
        margin-bottom: 10px;
        list-style: none;
    }
    .question {
        font-weight: bold;
    }
    .content {
        color: red;
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
</style>
