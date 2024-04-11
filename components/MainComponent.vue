<template>
    <main>
        <div class="container py-4">
            <h3 class="text-white">-->content goes here<--</h3>
            <div class="row">
                <div class="col-12 col-md-3 col-lg-2 " v-for="(element, index) in comics" :key="index">
                    <CardComponent :image="element.thumb" :type="element.type" :title="element.series" />
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


</style>