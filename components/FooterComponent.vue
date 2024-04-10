<template>
    <div>
        <FooterTop/>
        <FooterMid/>
        <Footerbottom/>
    </div>
</template>

<script>
import FooterTop from '../components/FooterTop.vue';
import FooterMid from '../components/FooterMid.vue';
import Footerbottom from '../components/FooterBottom.vue';
    export default {
        name: 'FooterComponent',
        components: {
            FooterTop,FooterMid,Footerbottom
        }
    }
</script>

<style lang="scss" scoped>

</style>