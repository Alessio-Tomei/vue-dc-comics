<template>
<main>
    <div class="jumbotron">
        <img src="../assets/img/jumbotron.jpg" alt="">
    </div>
    <div class="container">
        <section class="current-series">
            <p class="section-title">CURRENT SERIES</p>
            <div class="comics-container">
                <ComicsBox 
                v-for="(comics, index) in comicsArray"
                :key="index"
                :comicsObj="comics"/>
            </div>
        </section>
    </div>
</main>
</template>

<script>
import comicsList from '../data/comics-list';
import ComicsBox from './ComicsBox.vue'

export default {
    name: 'Main',
    components: {
        ComicsBox,
    },
    data() {
        return {
            comicsArray: comicsList,
        } 
    }
}
</script>

<style lang="scss">
@import '../assets/style/partials/variables.scss';

main {
    background-color: $darkColor;
    color: $lightColor;
}

.jumbotron {
    height: 500px;
    overflow: hidden;
}

.jumbotron img {
    width: 100%;
}

.container {
    .current-series {
        padding: $sectionPadding;
        position: relative;
        .section-title {
            font-weight: bold;
            padding: 10px 30px;
            background-color: $dcMainColor;
            position: absolute;
            top: -20px;
            left: 0;
        }
        .comics-container {
            margin: 0 auto;
            max-width: 1483px;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-evenly;
        }
    }
}
</style>