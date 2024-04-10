<template>
   <div class="container d-flex justify-content-between align-items-center p-4 ">
        <div>
            <img src="../public/img/dc-logo.png" alt="">
        </div>
        <div>
           <ul>
               <li v-for="(element, index) in menu" :key="index"><a :href="element.url">{{ element.name }}</a></li>
           </ul>
        </div>
   </div>
</template>

<script>
    export default {
       name:'HeaderComponent',
       data(){
           return{
                menu: [
                    {
                        name: 'characters',
                        url: '#',
                    },
                    {
                        name: 'comics',
                        url: '#',
                    },
                    {
                        name: 'movies',
                        url: '#',
                    },
                    {
                        name: 'tv',
                        url: '#',
                    },
                    {
                        name: 'games',
                        url: '#',
                    },
                    {
                        name: 'collectibles',
                        url: '#',
                    },
                    {
                        name: 'videos',
                        url: '#',
                    },
                    {
                        name: 'fan',
                        url: '#',
                    },
                    {
                        name: 'news',
                        url: '#',
                    },
                    {
                        name: 'shop',
                        url: '#',
                    },
                    	
                ]

           }
       }
    }
</script>

<style lang="scss" scoped>
    ul {
        list-style: none;
        display: flex;
        justify-content: center;
        
         li {
            color: black;
            margin: 0 10px;

            a {
                text-decoration: none;
                color: black;
                font-weight: 600;
            }
        }
    }

</style>