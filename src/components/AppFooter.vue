<script>
    export default {
        name: 'AppFooter'
    }
</script>

<template>
    <footer>
        <div class="container">
            <div class="logo">
            <img src="../assets/img/logo-sidearea-1.png" alt="logo">
                <div>Let's Get Creative</div>
            </div>
            <div class="social-links">
                <div>Stay in touch with us</div> 
                <div class="social">
                </div>
            </div>
        </div>  
    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/style/partials/commons.scss' as *;
@use '../assets/style/partials/colors.scss' as *;
footer{
    background-color: $bg-mint;
    width: 100%;
    padding-top: 50px;
    padding-bottom: 60px;
    .container{
        display: flex;
        justify-content: flex-start;
        align-items: center;
        font-size: 14px;
        .logo{
            line-height: 25px;
            margin-left: 100px;
            margin-right: 140px;
        }
        .social-links{
            text-align: center;
            line-height: 30px;
        }
    
    }
}
</style>