<script>
export default {
    name: "AppTitle",
    data(){
        return {
            message: "La mia prima app con Vite!"
        }
    }
}
</script>

<template>
  <div class="title">
    {{ message }}
  </div>
</template>

<style scoped>
    .title{
        padding: 50px;
        background-color: antiquewhite;
        color: rgb(22, 137, 183);
        font-size: 50px;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
</style>