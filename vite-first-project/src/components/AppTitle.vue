<script>
export default {
    data(){
        return {
            message: 'La mia prima app con Vite!'
        }
    }
}


</script>

<template>

    <div>
        <h1 class="title">
            {{ message }}
        </h1>
    </div>

</template>


<style scoped>
.title {
    color: red;
    border: 2px solid red;
}


</style>