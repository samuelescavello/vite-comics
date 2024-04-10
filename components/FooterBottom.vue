<template>
    <div id="bottom">
        <div class="container d-flex justify-content-between">
            <div class="bottone text-center text-uppercase">
                sing-up now!
            </div>
            <div>
                <h5 class="text-uppercase ">
                    follow us
                </h5>
                <!-- <ul>
                    <li>
                        <a>
                            
                        </a>
                    </li>
                </ul> -->
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'footerBottom',
        Data(){
            return{
                images: ['/img/footer-facebook.png', '/img/footer-twitter.png', '/img/footer-youtube.png', '/img/footer-pinterest.png', '/img/footer-periscope.png']
            }
        }
    }
</script>

<style lang="scss" scoped>
#bottom {
    background-color: #303030;
    color: white;
    padding: 30px;
}

.bottone{
    border: 2px solid #0282F9;
    width: 150px;
    padding: 10px;
}

h5{
    padding-top: 10px;
    color: #0282F9;
}
   
</style>