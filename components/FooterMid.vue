<template>
    <div id="mid" class="d-flex">
        <div class="d-flex container ">

            <div id="left" class=" d-flex">
                <ul>
                    <h4 class="text-uppercase pb-3 ">dc comics</h4>
                    <li v-for=" (element, index) in listOne" :key="index">
                        <a href="#">{{element.testoOne}}</a>
                    </li>
                </ul>
                <ul>
                    <h4 class="text-uppercase pb-3 ">dc</h4>
                    <li v-for=" (element, index) in listTwo" :key="index">
                        <a href="#">{{element.testoTwo}}</a>
                    </li>
                </ul>
                <ul>
                    <h4 class="text-uppercase pb-3 ">sites</h4>
                    <li v-for=" (element, index) in listThree" :key="index">
                        <a href="#">{{element.testoThree}}</a>
                    </li>
                </ul>
            </div>
            <div id="right">
                <!-- <img src="../public/img/dc-logo-bg.png" alt="#"> -->
            </div>

        </div>
    </div>
</template>

<script>
    export default {
        name: 'footerMid',
        data (){
            return {
                listOne: [
                    {
                        testoOne: 'Characters',
                    },
                    {
                        testoOne: 'Comics',
                    },
                    {
                        testoOne: 'Movies',
                    },
                    {
                        testoOne: 'Tv',
                    },
                    {
                        testoOne: 'Games',
                    },
                    {
                        testoOne: 'Videos',
                    },
                    {
                        testoOne: 'News',
                    }
                ],
                listTwo: [
                    {
                        testoTwo:'Terms of use',
                    },
                    {
                        testoTwo:'Privacy policy (new)',
                    },
                    {
                        testoTwo:'Ad choices',
                    },
                    {
                        testoTwo:'Advertising',
                    },
                    {
                        testoTwo:'Jobs',
                    },
                    {
                        testoTwo:'Subscriptions',
                    },
                    {
                        testoTwo:'Talent workshops',
                    },
                    {
                        testoTwo:'CPSC certificates',
                    },
                    {
                        testoTwo:'Ratings',
                    },
                    {
                        testoTwo:'Shop help',
                    },
                    {
                        testoTwo:'Contact us',
                    }
                ],
                listThree : [
                    {
                        testoThree:'DC',
                    },
                    {
                        testoThree:'MAD Magazine',
                    },
                    {
                        testoThree:'DC Kids',
                    },
                    {
                        testoThree:'DC Universe',
                    },
                    {
                        testoThree:'DC Power Visa',
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>

    #mid {
        display: flex;
        background-image: url(../public/img/footer-bg.jpg);
        background-repeat:no-repeat ;
        background-size: cover;
    }

    #left {
        width: 50%;
        color: white;
        
    }

    #right {
        width: 50%;
        background-image: url(../public/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-size: cover;
    }

    .debug {
        border: 1px solid red;
    }

    ul {
        list-style: none;
        margin-top: 50px;

        a {
            text-decoration: none;
            color: lightgray;
         }
        
    }

    a:hover {
        color: white;
    }
</style>