<template>
    <div id="bottom">
        <div class="container d-flex justify-content-between">
            <div class="bottone text-center text-uppercase">
                <a href="#">sing-up now!</a>
            </div>
            <div class="d-flex ">
                <div id="follow">
                    <h5 class="text-uppercase ">
                    follow us
                    </h5>
                </div>
                
                <ul class="d-flex">
                    <li><a href="#"><img src="../public/img/footer-facebook.png" alt="foto"></a></li>
                    <li><a href="#"><img src="../public/img/footer-twitter.png" alt="foto"></a></li>
                    <li><a href="#"><img src="../public/img/footer-youtube.png" alt="foto"></a></li>
                    <li><a href="#"><img src="../public/img/footer-pinterest.png" alt="foto"></a></li>
                    <li><a href="#"><img src="../public/img/footer-periscope.png" alt="foto"></a></li>
                </ul>
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
    padding: 10px;
    height: 50px;

    &:hover{
        background-color: #0282F9;
    }

    a{
        text-decoration: none;
        color: white;

    }
}

h5{
    padding-top: 10px;
    color: #0282F9;
    cursor: pointer;

    &:hover{
        color: white;
    }
}

ul{
    list-style: none;
    padding-top: 5px;

    li{
        margin: 0 10px;
    }
}

</style>