<template>
  <div class="back-top">
    <img src="@/assets/img/common/top.png" alt="">
  </div>
</template>
<script>
export default
{
  name:'BackTop',
  // methods: {
  //   backClick(){
  //     console.log('回到顶部')
  //   }
  // }
}
</script>
<style scoped>
 .back-top{
   position: fixed;
   right: 10px;
   bottom:60px
 }
 .back-top img{
   width: 60px;
   height: 60px;
 }
</style>