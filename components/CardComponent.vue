<template>
    <div>
        <img :src="image" :alt="type" class="img-fluid v-100">
    </div>
    <div>
       <h6 class="text-uppercase p-2 ">{{ title }}</h6>
    </div>
</template>

<script>
    export default {
        name: 'CardComponent',
        props:[
            'image',
            'type',
            'title'
        ]
    }
</script>

<style lang="scss" scoped>
    img {
        // width: 200px;
        // height: 230px;
        min-height: 300px;
    }
</style>