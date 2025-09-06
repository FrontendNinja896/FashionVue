<script>
import Header from './components/Header.vue'
import Vehicle from './components/Vehicle.vue'
import Articles from './components/Articles.vue'
import FollowIns from './components/FollowIns.vue'
import Pagination from './components/Pagination.vue'
export default{
  components:{Header,Vehicle,Articles,FollowIns,Pagination},
  data(){
    return{
      ArrayHrefs:["Home","Recipes","Article","Contact","Purchase"],
      ArrayNews:[
        {pathImg:"./src/assets/img/Tourism.svg",category:"Tourism",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"},
        {pathImg:"./src/assets/img/Fashion.svg",category:"Fashion",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"},
        {pathImg:"./src/assets/img/Clothes.svg",category:"Clothes",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"},
        {pathImg:"./src/assets/img/Autumn.svg",category:"Autumn",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"},
        {pathImg:"./src/assets/img/Summer.svg",category:"Summer",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"}
      ],
      ArraySecondNews:[
        {pathImg:"./src/assets/img/Sport.svg",category:"Sport",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"},
        {pathImg:"./src/assets/img/ClothesSecond.svg",category:"Clothes",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"},
        {pathImg:"./src/assets/img/FashionSecond.svg",category:"Fashion",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"},
        {pathImg:"./src/assets/img/ClothesThird.svg",category:"Clothes",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"},
        {pathImg:"./src/assets/img/SummerSecond.svg",category:"Summer",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"}
      ],
      ImageArray:[
        {pathImg:"./src/assets/img/Widget1.svg"},
        {pathImg:"./src/assets/img/Widget2.svg"},
        {pathImg:"./src/assets/img/Widget3.svg"},
        {pathImg:"./src/assets/img/Widget4.svg"},
        {pathImg:"./src/assets/img/Widget5.svg"},
        {pathImg:"./src/assets/img/Widget6.svg"}
      ],
      ArrayPosts:[
        {pathImg:"./src/assets/img/Jeans.svg",category:"Jeans",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"},
        {pathImg:"./src/assets/img/City.svg",category:"City",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"},
        {pathImg:"./src/assets/img/Photography.svg",category:"Photography",description:"One of Saturn’s largest rings may be newer than anyone",DopInfo:"June 6, 2019    By Rickie Baroch    4 comments"},
      ],
      ArrayCategories:[
        {category:"Fashion"},
        {category:"Style & clothes"},
        {category:"Minimalism"},
        {category:"Black & White"},
        {category:"Modern Clothes"}
      ]
    }
  }
}
</script>

<template>
  <Header :Links="ArrayHrefs"></Header>
  <Vehicle></Vehicle>
  <Articles :NewsArray="ArrayNews" :NewsArraySecond="ArraySecondNews" :Posts="ArrayPosts" :Categories="ArrayCategories"></Articles>
  <Pagination></Pagination>
  <FollowIns :Images="ImageArray" ></FollowIns>
</template>

<style scoped></style>