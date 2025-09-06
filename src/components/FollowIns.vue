<script>
export default{
    props:{
        Images:{
            type:Array,
            required:true
        }
    }
}
</script>

<template>
  <p class="text-center fs-2 fw-bolder mt-5">Follow our @instagram_name</p>
  <div v-for="(el,index) in Images" :key="index" class="d-flex flex-row  justify-content-center mb-3">
        <img :src="el.pathImg" alt="">
  </div>
</template>

<style scoped>

</style>