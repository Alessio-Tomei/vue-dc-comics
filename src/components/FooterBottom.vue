<template>
<div class="footer-bottom">
    <div class="container">
        <div class="button">
            SING UP NOW!
        </div>
        <div class="social">
            <span>FOLLOW US</span>
            <img src="../assets/img/footer-facebook.png" alt="">
            <img src="../assets/img/footer-twitter.png" alt="">
            <img src="../assets/img/footer-youtube.png" alt="">
            <img src="../assets/img/footer-pinterest.png" alt="">
            <img src="../assets/img/footer-periscope.png" alt="">
        </div>
    </div>
</div>
</template>

<script>
export default {
    name: 'FooterBottom',
}
</script>

<style lang="scss">
@import '../assets/style/partials/variables.scss';

.footer-bottom {
    background-color: rgb(32, 32, 32);
    height: 80px;
    .container {
        display: flex;
        height: 100%;
        justify-content: space-between;
        align-items: center;
        .button {
            padding: 10px;
            border: 2px solid $dcMainColor;
            color: $lightColor;
        }
        .social {
            display: flex;
            align-items: center;
            & > * {
                margin-left: 20px;
            }
            span {
                color: $dcMainColor;
                font-weight: bold;
            }
        }
    }
}

</style>