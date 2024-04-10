<template>
    <div id="top">
        <div class="container d-flex justify-content-space-between py-5 ">
            <ul>
                <li v-for="(element, index) in menuFooter" :key="index"><a href="#"><img :src="element.img" alt="#"><span class="text-uppercase">{{ element.testo }}</span></a></li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'footerTop',
        data (){
            return {
                menuFooter: [
                    {
                        img : '../public/img/buy-comics-digital-comics.png',
                        testo : 'Digital Comics'
                    },
                    {
                        img : '../public/img/buy-comics-merchandise.png',
                        testo : 'Dc Merchandise'
                    },
                    {
                        img : '../public/img/buy-comics-subscriptions.png',
                        testo : 'Subscription'
                    },
                    {
                        img : '../public/img/buy-comics-shop-locator.png',
                        testo : 'Comic Shop Locator'
                    },
                    {
                        img : '../public/img/buy-dc-power-visa.svg',
                        testo : 'Dc Power Visa'
                    },
                   
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    #top {
        background-color: #0282F9;
    }
    img {
        width: 50px;
        height: 60px;
    }

    ul {
        list-style: none;
        display: flex;
        
         li {
            margin: 0 10px;
            padding-right: 40px;

            a {
                text-decoration: none;
                color: white;
                font-weight: 600;
            }
        }
    }

    span {
        padding-left: 10px;
    }

</style>