<template>

<header>
 <img alt="Vue logo" src="../assets/images/dc-logo.png">
 <nav>
   <ul>
     <li  
        v-for="(items, index) in links" 
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
  data(){
    return{
      links:[
        {
          testo:"characters",
          link:"",
          active: false
        },
        {
          testo:"comics",
          link:"",
          active: true
        },
        {
          testo:"movies",
          link:"",
          active: false
        },
        {
          testo:"tv",
          link:"",
          active: false
        },
        {
          testo:"games",
          link:"",
          active: false
        },
        {
          testo:"collectibles",
          link:"",
          active: false
        },
        {
          testo:"videos",
          link:"",
          active: false
        },
        {
          testo:"fans",
          link:"",
          active: false
        },
        {
          testo:"news",
          link:"",
          active: false
        },
        {
          testo:"shop",
          link:"",
          active: false
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../style/variables';
@import '../style/generals';

header{
  width: $width;
  margin: 0 auto;
  font-weight:600;
  font-size: $main-font-size;
  height: $line-height;
}
ul{
  float: right;
}
li{
  padding: 0 15px;
  text-transform: uppercase ;
  line-height: $line-height;
  list-style: none;
  float: left;
}
img{
  margin: 15px 0;
  height: 50px;
  float: left;
}

.active {
  background-color: $bg-active;
}

</style>
