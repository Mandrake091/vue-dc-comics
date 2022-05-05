<template>

<header>
 <img alt="Dc logo" src="/images/dc-logo.png">
 <nav>
   <ul>
     <li  
        v-for="(items, index) in link" 
        :key="index" 
        :class="{'active' : items.active}"> {{items.testo}}
     </li>
   </ul>
 </nav>
 </header> 
 
</template>

<script>

export default {
  name: 'AppHeader',
  props:['link']
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../style/variables';
@import '../style/generals';

header{
  justify-content: space-between;
  display: flex;
  width: $width;
  margin: 0 auto;
  font-weight:600;
  font-size: $main-font-size;
}
li{
  padding: 0 15px;
  text-transform: uppercase ;
  line-height: 100px;
  list-style: none;
  float: left;
}
img{
  margin: 15px 0;
  height: 70px;
  float: left;
}

.active {
  background-color: $bg-active;
}

</style>
