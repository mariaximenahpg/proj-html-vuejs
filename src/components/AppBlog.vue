<script>
import {blogPosts} from '../data/arrays.js'
import AppCardBlog from './AppCardBlog.vue';
    export default {
    name: "AppBlog",
    components: { AppCardBlog },
    data(){
        return {
            posts: blogPosts,
        }
    }
}
</script>

<template>
    <section id="blog">
        <div class="blog-container">
            <div class="box">
                <div class="row">
                   <AppCardBlog v-for="(item,index) in posts" :key="index" :image="item"/>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/style/partials/commons.scss' as *;
@use '../assets/style/partials/colors.scss' as *;
#blog{
    padding: 70px 0;
}
.box{
    width: 100%;
    .row{
        display: flex;
        flex-flow: row nowrap;
        justify-content: center;
        align-items: center;
        width: 100%;    
    }
}
</style>