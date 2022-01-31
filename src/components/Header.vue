<template>
<header>
    <div class="container">
        <div class="container-logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li v-for="(navElement, index) in navTabs" :key="index">
                    <a href="" :class="{'active' : navElement.current}"><span>{{navElement.tabName}}</span></a>
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
        navTabs: [
            {
                tabName: 'characters',
                current: false,
            },
            {
                tabName: 'comics',
                current: true,
            },
            {
                tabName: 'movie',
                current: false,
            },
            {
                tabName: 'tv',
                current: false,
            },
            {
                tabName: 'games',
                current: false,
            },
            {
                tabName: 'collectibles',
                current: false,
            },
            {
                tabName: 'videos',
                current: false,
            },
            {
                tabName: 'fans',
                current: false,
            },
            {
                tabName: 'news',
                current: false,
            },
            {
                tabName: 'shop',
                current: false,
            },
            
        ] 
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
    width:40%;
}

nav {
    width: 60%;
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
        font-size: 0.7rem;
        color: $darkColor;
        text-transform: uppercase;
        &.active, &:hover {
            box-shadow: inset 0px -6px 0px 0px $dcMainColor;
        }
    }
}
</style>