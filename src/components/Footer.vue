<template>
<footer>
    <FooterTop/>
    <FooterMid/>
    <FooterBottom/>
</footer>
</template>

<script>
import FooterTop from './FooterTop.vue';
import FooterMid from './FooterMid.vue';
import FooterBottom from './FooterBottom.vue';

export default {
    name: 'Footer',
    components: {
        FooterTop,
        FooterMid,
        FooterBottom
    }
}
</script>

<style lang="scss">

</style>