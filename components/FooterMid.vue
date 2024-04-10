<template>
    <div id="mid" class="d-flex">
        <div class="d-flex container ">

            <div id="left" class=" debug d-flex">
                <ul>
                    <h4 class="text-uppercase pb-3 ">dc comics</h4>
                    <li v-for=" (element, index) in listOne" :key="index">
                        {{element.testoOne}}
                    </li>
                    
                    <ul>
                        <li>d</li>
                    </ul>
                </ul>
                <ul>
                    <h4 class="text-uppercase pb-3 ">dc</h4>
                    <li v-for=" (element, index) in listTwo" :key="index">
                        {{element.testoTwo}}
                    </li>
                </ul>
                <ul>
                    <h4 class="text-uppercase pb-3 ">sites</h4>
                    <li v-for=" (element, index) in listThree" :key="index">
                        {{element.testoThree}}
                    </li>
                </ul>
            </div>
            <div id="right" class="debug">
                <img src="../public/img/dc-logo-bg.png" alt="#">
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
                        testoTwo:'terms of use',
                    },
                    {
                        testoTwo:'privacy policy (new)',
                    },
                    {
                        testoTwo:'ad choices',
                    },
                    {
                        testoTwo:'advertising',
                    },
                    {
                        testoTwo:'jobs',
                    },
                    {
                        testoTwo:'subscriptions',
                    },
                    {
                        testoTwo:'talent workshops',
                    },
                    {
                        testoTwo:'CPSC certificates',
                    },
                    {
                        testoTwo:'ratings',
                    },
                    {
                        testoTwo:'shop help',
                    },
                    {
                        testoTwo:'contact us',
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
        background-size: 100%;
    }

    #left {
        width: 50%;
        color: white;
        
    }

    #right {
        width: 50%;

    }

    .debug {
        border: 1px solid red;
    }

    ul {
        list-style: none;
        margin-top: 50px;

        li {
            color: lightgray;
        }
    }
</style>