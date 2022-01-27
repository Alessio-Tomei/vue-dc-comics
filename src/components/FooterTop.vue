<template>
<div class="footer-top">
    <div class="container">
        <div class="icon-link">
            <a href="">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span>digital comics</span>
            </a>
        </div>
        <div class="icon-link">
            <a href="">
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                <span>dc merchandise</span>
            </a>
        </div>
        <div class="icon-link">
            <a href="">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                <span>subscription</span>
            </a>
        </div>
        <div class="icon-link">
            <a href="">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <span>comics shop locator</span>
            </a>
        </div>
        <div class="icon-link">
            <a href="">
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                <span>dc power visa</span>
            </a>
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'FooterTop',
}
</script>

<style lang="scss">
@import '../assets/style/partials/variables.scss';

.footer-top {
    padding: $sectionPadding;
    background-color: $dcMainColor;
}

.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.icon-link {
    width: 20%;
     a {
        width: max-content;
        display: flex;
        align-items: center;
        img {
            height: 65px;
            margin-right: 20px;
        }
        span {
            color: $lightColor;
            text-transform: uppercase;
        }
    }
}    

</style>