<script setup>
// import { RouterLink, RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
// import HeaderComponent from './components/Header/HeaderComponent.vue';
import MainComponent from './components/MainComponent.vue';
import AuthorSweets from './components/AuthorSweets.vue'
import TopDeserts from './components/TopDeserts.vue'
import FillingsComponentVue from './components/FillingsComponent.vue';
import OrderDetailsVue from './components/OrderDetails.vue';
import TopQuestionsVue from './components/TopQuestions.vue';
import FooterComponentVue from './components/FooterComponent.vue';
</script>

<template>
  <header>
    <MainComponent />
    <AuthorSweets />
    <TopDeserts />
    <FillingsComponentVue />
    <OrderDetailsVue />
    <TopQuestionsVue />
    <FooterComponentVue />



      <!-- <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav> -->
  </header>

  <!-- <RouterView /> -->
</template>

<style scoped>
  .app{
    background-color: antiquewhite;
  }
header {
  line-height: 1.5;
  max-height: 100vh;
}





@media (min-width: 1024px) {
  
}
</style>
