<script lang="ts">
export default {
    name: "AppHero",
    data(){
        return {
            imageName: "vite.svg"
        }
    },
    methods: {
        getImagePath: function(img){
            return new URL (`/public/${img}`, import.meta.url).href;
        }
    }
}
</script>

<template>
  <div>
    <img :src="getImagePath(imageName)" alt="image not found" class="jumboImg">
  </div>
</template>

<style scoped>
    .jumboImg{
        display: block;
        margin-left: auto;
        margin-right: auto;
        width: 50%;
    }
</style>