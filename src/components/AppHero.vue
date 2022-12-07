<script>
export default{
    name: "AppHero",
};
</script>

<template>
    <div class="hero">
        <button class="chevron left"><i class="fa-solid fa-chevron-left"></i></button>
        <div class="container">
            <div class="carousel">
                <div class="carousel-text">
                    <h1>Devotion that<br>never <span class="cursive">ends</span></h1>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit reiciendis sint, ducimus quo alias ipsam labore tempore minima soluta blanditiis.</p>
                    <button class="btn">Read More</button>
                </div>
                <div class="carousel-img">
                    <img src="../assets/img/h-2-slider-img-15.png" alt="">
                    <img src="../assets/img/h-2-slider-img-16.png" alt="">
                </div>

            </div>

        </div>
        <button class="chevron right"><i class="fa-solid fa-chevron-right"></i></button>
        

    </div>
</template>

<style lang="scss" scoped>
@use '../assets/style/partials/commons.scss' as *;
@use '../assets/style/partials/colors.scss' as *;
.hero{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 30px;
    margin-bottom: 60px;
    .container{
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        width: 90%;
        margin: 0 auto;
        height: 300px;
        overflow: hidden;
        position: relative;
        .carousel{
            display: flex;
            justify-content: flex-end;
            align-items: center;
            height: 100%;
            .carousel-text{
                width: 40%;
                height: 100%;
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: flex-start;
                padding-left: 165px;
                font-family: 'Lato', sans-serif;
                h1{
                        font-size: 40px;
                        font-weight: 300;
                        line-height: 40px;
                        
                }
                .cursive{
                    font-family: 'Satisfy', cursive;
                }
                p{
                    color: $text-gray;
                    line-height: 15px;
                    margin: 30px 0;
                    font-size: 14px;
                    max-width: 580px
                    
                }
                .btn{
                    border: 2px solid $bg-pink;
                    background-color: transparent;
                    margin-top: 8px;
                    position: relative;
                    padding: 10px 20px;
                }

            }
            .carousel-img{
                display: flex;
                width: 40%;
                height: 250px;
                margin-left: 30px;

            }
        }

    }
}
</style>