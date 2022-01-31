<template>
<div class="comics-box">
    <div class="img-container">
        <img :src="comicsObj.thumb" alt="">
    </div>
    <p>{{comicsObj.series}}</p>
</div>
</template>

<script>
export default {
    name: 'ComicsBox',
    props: {
        comicsObj: Object,
    },
}
</script>

<style lang="scss">
$boxDimension: 192px;

.comics-box {
    padding: 20px 10px;
    .img-container {
        width: $boxDimension;
        height: $boxDimension;
        overflow: hidden;
        img {
            width: 100%;
        }
    }
    p {
        margin-top: 10px;
        width: $boxDimension;
    }
}

</style>