<template>
    <div class="single-card">
        <img :src="comicObject.thumb" :alt="comicObject.series">
        <h4>{{ comicObject.series }}</h4>
    </div>
</template>
<script>


export default {
    name: "comicsItem",
    props: ['comicObject']
}
</script>

<style lang="scss" scoped>
@import '../style/variables';

    
.single-card{
    width: calc((100% / 6) - 10px); 
    margin: 4px;
    img{
        width: 100%;
        height: auto;
    }
    h4{
        color: white;
        padding: 10px  0;
    }
}



</style>