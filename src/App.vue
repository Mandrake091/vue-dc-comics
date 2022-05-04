<template>

  <div id="app">
    <div class="container">

   
      <header>
        <app-header/> 
      </header>

      <main>
        <app-grid/>
      </main>
    
      <app-footer/>

   </div> 
  </div>
</template>

<script>

import AppHeader from './components/AppHeader.vue';
import AppGrid from './components/AppGrid.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  name: 'App',
  components: {
    AppHeader,
    AppGrid,
    AppFooter
  }
,
    AppFooter}
</script>

<style lang="scss">
@import './style/variables';
@import './style/generals';

.container{
  
  margin: 0 auto;
}

</style>
