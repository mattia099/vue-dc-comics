<template>
    <div class="comicsCard">
        <img :src="element.thumb" alt="">
        <h5>{{ element.series }}</h5>
    </div>
</template>


<script>

export default {
    props:{
        element : Object
    },
    created(){
        console.log(this.element)
    }
}
</script>


<style lang="scss" scoped>
    .comicsCard{
        width: 180px;
        img{
        width: 100%;
        height: 180px;
        }
    }
    
</style>