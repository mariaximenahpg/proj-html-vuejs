<script>
    export default {
        name: 'AppPortfolio'
    }
</script>

<template>
    <section class="portfolio">
        <div class="portfolio-container">
            <div class="col">
                <div class="box">
                    <img src="../assets/img/h-2-port-img-1.jpg" alt="">
                    <div class="content">
                        <h4>All these illustrations</h4>
                    </div>
                    <div id="cursive">Illustration</div>
                </div>
                <div class="box">
                    <img src="../assets/img/h-2-port-img-2.jpg" alt="">
                </div>
                <div class="box">
                    <img src="../assets/img/h-2-port-img-3.jpg" alt="">
                </div>
            </div>
            <div class="col">
                <div class="box">
                    <img src="../assets/img/h-2-port-img-4.jpg" alt="">
                </div>
                <div class="box">
                    <img src="../assets/img/h-2-port-img-5.jpg" alt="">
                </div>
                <div class="box">
                    <img src="../assets/img/h-2-port-img-6.jpg" alt="">
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/style/partials/commons.scss' as *;
@use '../assets/style/partials/colors.scss' as *;
.portfolio-container{
    width: 100%;
    font-family: 'Lato', sans-serif;
    .col{
        display: flex;
        flex-flow: row nowrap;
        justify-content: space-between;
        align-items: center;

        .box{
            position: relative;
            cursor: pointer;
            overflow: hidden;
                img{
                    transform: scale(1);
                    max-width: 100%;
                }
                h4{
                    font-weight: 500;
                    font-size: 25px;
                    padding-bottom: 8px;
                    opacity: 0;
                } 
                .content{
                    background-color: $bg-white ;
                    padding: 20px;
                    padding-bottom: 44px;
                    position: absolute;
                    top: 42%;
                    left: -100%;
                    opacity: 0;
                }
            }
            .box:hover .content{
                    left: 0;
                    opacity: 1;
            }
            #cursive{
                    font-size: 14px;
                    font-weight: 200;
                    font-family: 'Satisfy', cursive;
                    margin-top: 12px;
                    position: absolute;
                    top: 52%;
                    left: -100%;
                    z-index: 1;
            }
            .box:hover #cursive{
                left: 24px;
            }
            .box:hover h4{
                opacity: 1;
            }
        

        }
}

</style>

