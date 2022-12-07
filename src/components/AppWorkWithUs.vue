<script>
    export default {
        name: 'AppWorkWithUs'
    }
</script>

<template>
    <section id="workWith">
        <h2>Want to work with us? Send us <span id="cursive">a message!</span></h2>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis voluptate laborum aliquid sed rerum dolorem natus accusamus amet. Architecto nam et ipsa sint suscipit? Dolorum voluptas placeat dicta blanditiis esse.</p>
        <button class="btn">CONTACT</button>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/style/partials/commons.scss' as *;
@use '../assets/style/partials/colors.scss' as *;
#workWith{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 550px;
    background-image: url(../assets/img/h-2-background-1.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    text-align: center;
    font-family: 'Lato', sans-serif;
    h2{
        font-weight: 100;
        font-size: 45px;
    }
    #cursive{
        font-family: 'Satisfy', cursive;
        font-size: 45px;
    }
   
    p{
        width: 70%;
        font-size: 14px;
        padding:23px;
        padding-bottom: 30px;
        font-weight: 100;
        color: $text-gray;
    }
    button{
        padding: 12px 40px;
        background-color: $bg-mint;
        position: relative;
        &:hover{
            color: $bg-white;
            background-color: $bg-pink;
        }
    }
}


</style>