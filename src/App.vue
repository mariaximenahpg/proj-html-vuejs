<script>
import AppHeader from'./components/AppHeader.vue';
import AppHero from'./components/AppHero.vue';
import AppPortfolio from'./components/AppPortfolio.vue';
import AppWorkingProcess from'./components/AppWorkingProcess.vue';
import AppWorkWithUs from'./components/AppWorkWithUs.vue';
import AppBlog from'./components/AppBlog.vue';
import AppFooter from'./components/AppFooter.vue';
export default {
  components:{
    AppHeader,
    AppHero,
    AppPortfolio,
    AppWorkingProcess,
    AppWorkWithUs,
    AppBlog,
    AppFooter,

  }, 
    data(){
      return{
      }
    },
};
</script>

<template>
  <AppHeader/>
  <main>
    <AppHero/>
    <AppPortfolio/>
    <AppWorkingProcess/>
    <AppWorkWithUs/>
    <AppBlog/>

  </main>
  <footer>
    <AppFooter/>
  </footer>
</template>