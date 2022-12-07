<script>
    export default {
        name: 'AppCardBlog',
        props:[
           
            'image'
        ],
    }
</script>

<template>
    <div class="card">
        <div class="date">
            <img src="" alt="">
            <div class="day">07</div>
            <div class="month">May ' 19'</div>
        </div>
        <div class="blog-image">
             <img :src="image.img" alt="">
        </div>
        <h4><span>{{image.title}}</span></h4>
        <div class="author">{{image.credits}}</div>
    </div>
</template>

<style lang="scss" scoped>
@use '../assets/style/partials/commons.scss' as *;
@use '../assets/style/partials/colors.scss' as *;
.card{
        display: flex;
        width: calc(100% / 3);
        padding: 0 14px;
        position: relative;
        // sistemare array img non le rileva
    }
</style>