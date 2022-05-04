<template>

<footer>
    <h1>Sono il footer!</h1>
   
 </footer> 

</template>

<script>
export default {
  name: 'AppFooter'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import '../style/variables';
@import '../style/generals';

footer{
    width: $width;
    margin: 0 auto;
}

h1{
 
  color: $bg-active;
  font-weight: 400;
}

</style>
