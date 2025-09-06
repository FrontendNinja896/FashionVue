<script>
export default{
    props:{
        NewsArray:{
            type:Array,
            required:true
        },
        NewsArraySecond:{
            type:Array,
            required:true
        },
        Posts:{
            type:Array,
            required:true
        },
        Categories:{
            type:Array,
            required:true
        }
    }
}
</script>

<template>
  <div class="d-flex flex-row justify-content-center mb-3">
  <div class="p-2">
        <div v-for="(el,index) in NewsArray" :key="index" class="card" style="width: 18rem;">
            <img :src="el.pathImg" class="card-img-top" alt="..."/>
            <div class="card-body">
                <p class="card-text">{{ el.category }}</p>
                <p>{{ el.description }}</p>
                <p>{{ el.DopInfo }}</p>
            </div>
        </div>
  </div>
  <div class="p-2">
        <div v-for="(el,index) in NewsArraySecond" :key="index" class="card" style="width: 18rem;">
                <img :src="el.pathImg" class="card-img-top" alt="..."/>
                <div class="card-body">
                    <p class="card-text">{{ el.category }}</p>
                    <p>{{ el.description }}</p>
                    <p>{{ el.DopInfo }}</p>
                </div>
        </div>
  </div>
  <div class="p-2">
        <button className="btn btn-primary btn-lg">Feautured Posts</button>
        <div v-for="(el,index) in Posts" :key="index" class="card" style="width: 18rem;">
                    <img :src="el.pathImg" class="card-img-top" alt="..."/>
                    <div class="card-body">
                        <p class="card-text">{{ el.category }}</p>
                        <p>{{ el.description }}</p>
                        <p>{{ el.DopInfo }}</p>
                    </div>
        </div>
        <button className="btn btn-primary btn-lg">Categories</button>
        <div v-for="(el,index) in Categories" :key="index">
            <p className="fs-2 text-primary">{{ el.category }}</p>
        </div>
  </div>
</div>
</template>

<style scoped>

</style>