<template>
<main>
    <div class="container">
        Content goes here 
    </div>
</main>
</template>

<script>
export default {
    name: 'Main'
}
</script>

<style lang="scss">
@import '../assets/style/partials/variables.scss';

main {
    padding: $sectionPadding;
    background-color: $darkColor;
    color: $lightColor;
}
</style>