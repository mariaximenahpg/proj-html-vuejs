<script>
import {headerNav} from '../data/arrays.js'
export default {
    name: 'AppHeader',
    data(){
        return{
            headerNavMenu: headerNav
        }
    }
}
</script>

<template>
    <header>
        <a href="#"><img class="logo" src="../assets/img/logo-sidearea-1.png" alt="logo"></a>
        <nav>
            <ul>
                <li v-for="(item,index) in headerNavMenu" :key="index">
                    <a href="#" :class="{'active' :item.active}" class="pageName">{{item.text}}</a>
                </li>
                <li>
                    <img class="grid-menu" src="../assets/svg/svg-1.svg" alt="menu grid icon">
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/style/partials/commons.scss' as *;
@use '../assets/style/partials/colors.scss' as *;
header{
    display: flex;
    flex-flow: row nowrap;
    justify-content: space-between;
    align-items: center;
    width: 95%;
    margin: 0 auto;
    height: 70px;
    padding-top: 50px;
    ul{
        display: flex;
        justify-content: center;
        align-items: center;
        font-family:  'Lato', sans-serif;;
        font-size: 14px;
        font-weight: bold;
        list-style: none;
        li a{
            display: inline-block;
            position: relative;
            text-decoration: none;
            color: $text;
            margin-left: 50px;
            letter-spacing: 1.5px;
        }
        .grid-menu{
            margin-left: 20px;
        }
        .pageName::after{
            display: block;
            width: 0%;
            height: 6px;
            background: $bg-pink;
            position: absolute;
            bottom: 0;
            z-index: -1; 
        }
        .pageName:hover::after{
            display: block;
            width: 100%;
            height: 6px;
            background: $bg-pink;
            position: absolute;
            bottom: 0;
            z-index: -1;
        } 
        .pageName.active::after{
            width: 100%;
        }
    }

}
</style>