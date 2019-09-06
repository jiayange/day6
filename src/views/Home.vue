<template>
  <div class="cont">
      <swiper :options="swiperOptions">
          <swiper-slide>1</swiper-slide>
          <swiper-slide>2</swiper-slide>
          <swiper-slide>3</swiper-slide>
      </swiper>
  </div>
</template>

<script>
export default {
   data(){
       return{
           swiperOptions:{
               autoplay:true
           }
       }
   }
}
</script>

<style lang="scss" scoped>
.cont{
    width: 100%;height: 100%;overflow: auto;
}
.swiper-container{
    width: 100%;height: 200px;background: pink;text-align: center;line-height: 200px;
}
</style>