<template>
    <main>
        <div id="jumbo"></div>
        <div class="container py-4">
            <div id="current"><h3 class="text-uppercase">current series</h3></div>
            <div class="row">
                <div class="col-12 col-md-3 col-lg-2 " v-for="(element, index) in comics" :key="index">
                    <CardComponent :image="element.thumb" :type="element.type" :title="element.series" />
                 </div>
             </div>
                 
             <div class="justify-content-center d-flex ">
                <div class="load text-center ">
                    <h3 class="text-uppercase">load more</h3>
                </div>
             </div>
        </div>
        
    </main>
</template>

<script>
import CardComponent from '../components/CardComponent.vue'
import {comics} from '../data/store.js'
    export default {
        name: 'MainComponent',
        components: {
            CardComponent
        },
        data () {
            return {
                comics
            }
        }
    }
</script>

<style lang="scss" scoped>
main {
    background-color: #1C1C1C;
    color: white;
}

#jumbo {
    height: 400px;
    background-image: url(../public/img/jumbotron.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

#current {
    background-color: #0282F9;
    padding: 8px;
    width: 235px;
    transform: translateY(-90%);
    cursor: pointer;

    &:hover {
        box-shadow:3px 3px 5px  #0282f986;
    }
}


.load{
    background-color: #0282F9;
    padding: 8px;
    width: 350px;
    cursor: pointer;

    &:hover {
        box-shadow:3px 3px 5px  #0282f986;
    }
}


</style>