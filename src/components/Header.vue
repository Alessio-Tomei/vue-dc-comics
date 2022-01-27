<template>
<header>
    <div class="container">
        <div class="container-logo">
        <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li>
                    <a href=""><span>characters</span></a>
                </li>
                <li>
                    <a href="" class="active"><span>comics</span></a>
                </li>
                <li>
                    <a href=""><span>movie</span></a>
                </li>
                <li>
                    <a href=""><span>tv</span></a>
                </li>
                <li>
                    <a href=""><span>games</span></a>
                </li>
                <li>
                    <a href=""><span>collectibles</span></a>
                </li>
                <li>
                    <a href=""><span>video</span></a>
                </li>
                <li>
                    <a href=""><span>fans</span></a>
                </li>
                <li>
                    <a href=""><span>news</span></a>
                </li>
                <li>
                    <a href=""><span>shop</span></a>
                </li>
            </ul>
        </nav>
    </div>
</header>
</template>

<script>
export default {
    name: 'Header',
    data() {
      return{
        
      }
    }
}
</script>

<style lang="scss">
@import '../assets/style/partials/variables.scss';

header {
    .container {
        height: 150px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
}

.container-logo {
    width:30%;
}

nav {
    width: 70%;
    height: 100%;
}

ul {
    height: 100%;
    width: 100%;
    display: flex;
    align-items: center;
    list-style: none;
}

li {
    width: 10%;
    height: 100%;
    a {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 100%;
        height: 100%;
        font-weight: bold;
        color: $darkColor;
        text-transform: uppercase;
        &.active, &:hover {
            box-shadow: inset 0px -6px 0px 0px $dcMainColor;
        }
    }
}
</style>