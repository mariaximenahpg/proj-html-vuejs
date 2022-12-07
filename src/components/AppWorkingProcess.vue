<script>
    export default {
        name: 'AppWorkingProcess'
    }
</script>

<template>
    <section id="steps">
        <div class="container">
            <h2>Working <span id="cursive">process</span></h2>
            <div class="box">
                <div class="row">
                    <div class="steps-col">
                        <div class="img">
                            <img src="" alt="">
                        </div>
                        <h3>First there is an idea</h3>
                        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                    </div>
                    <div class="steps-col">
                        <div class="img">
                            <img src="g" alt="">
                        </div>
                        <h3>First there is an idea</h3>
                        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                    </div>
                    <div class="steps-col">
                        <div class="img">
                            <img src="" alt="">
                        </div>
                        <h3>First there is an idea</h3>
                        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                    </div>
                    <div class="steps-col">
                        <div class="img">
                            <img src="" alt="">
                        </div>
                        <h3>First there is an idea</h3>
                        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                    </div>
                </div> 
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../assets/style/partials/commons.scss' as *;
@use '../assets/style/partials/colors.scss' as *;
#steps{
    text-align: center;
    margin-top: 100px;
    margin-bottom: 100px;
    font-family: 'Lato', sans-serif;
    h2{
        font-weight: 100;
        font-size: 45px;
    }
    #cursive{
        font-family: 'Satisfy', cursive;
        font-size: 45px;
    }

    .box{
        width:100%;
        margin-top: 30px;
    }
    .row{
        display: flex;
        flex-flow: row nowrap;
        justify-content: center;
        align-items: center;
    }
    .steps-col{
        flex-basis: calc(100% / 4);
        padding: 32px 4px;
   
        img{
            margin: 24px auto;
            width: 160px;
        }
        h3{
            font-size: 20px;
            font-weight: 400;
            margin-bottom: 14px;
        }
        
        p{
            font-size: 14px;
            width: 300px;
            margin: auto;
            font-weight: 100;
        }


    }
}
</style>