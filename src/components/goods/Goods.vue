<template>
  <div class="goods">
    <!-- 分类列表 -->
    <div class="menu-wrapper">
      
    </div>
    <!-- 商品列表 -->
    <div class="foods-wrapper">
      
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.goods{
  display: flex;
  position: absolute;
  top: 190px;
  bottom: 51px;
  overflow: hidden;
  width: 100%;
}

.goods .menu-wrapper{
  flex:0 0 85px;
  background: #f4f4f4;
}

.goods .foods-wrapper{
  flex:1;
  background: blue; 
}
</style>
