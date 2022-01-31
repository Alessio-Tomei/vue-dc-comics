<template>
<div class="footer-mid">
    <div class="container">
        <div class="links-container">
            <ul>
                <li>
                    <h2>titolo elenco</h2>
                </li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
            </ul>
            <ul>
                <li>
                    <h2>titolo elenco</h2>
                </li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
            </ul>
            <ul>
                <li>
                    <h2>titolo elenco</h2>
                </li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
            </ul>
            <ul>
                <li>
                    <h2>titolo elenco</h2>
                </li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
                <li>elemento elenco</li>
            </ul>
        </div>
        <div class="bg-logo">
            <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
    </div>
</div>
</template>

<script>
export default {
    name:'FooterMid',
}
</script>

<style lang="scss">
@import '../assets/style/partials/variables.scss';

.footer-mid {
    background-image: url("../assets/img/footer-bg.jpg");
        height: 482px;
    .container {
        overflow: hidden;
        height: 100%;
        .bg-logo img {
            height: 700px;
        }
        .links-container {
            padding-top: 30px;
            height: 100%;
            width: 100%;
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            align-content: flex-start;
            ul {
                height: max-content;
                width: 200px;
                display: flex;
                flex-direction: column;
                color: $lightColor;
                li {
                    padding-bottom: 5px;
                    width: max-content;
                }
            }
        }
    }
}
</style>