<template>
     <div>
        <img :src="thumb" :alt="type">
        <h3>{{series}}</h3>
    </div>
</template>

<script>
export default {
    name:'AppCard', 
    props:['thumb', 'series', 'type'] 
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
@import '../style/generals';
div{
    text-align: center;
    width: calc(100% / 6 - 40px) ;
    color: $font-white;
    font-size: $main-font-size;
}
img{
    width: 100%;
    object-fit: cover;
    object-position: top;
}


</style>