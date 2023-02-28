<script>
export default {
    data(){
        return {
            image: 'megatron.jpg',
        }
    },
    methods: {
        getImagePath(imagePath){
            return new URL(imagePath, import.meta.url).href;
        }
    }
}


</script>

<template>

    <div class="jumbotron">
        <img :src="getImagePath(`../assets/${image}`)">
    </div>

</template>


<style scoped>
img {
    max-width: 100%;
}
.jumbotron {
    margin: 0 auto;
    width: 75%;
    padding: 20px;
}


</style>