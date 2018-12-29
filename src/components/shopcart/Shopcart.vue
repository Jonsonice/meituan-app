<template>
  <div class="shopcart-wrapper">
    <!-- 底部左侧 -->
    <div class="content-left">
      <div class="logo-wrapper">
        <span class="icon-shopping_cart"></span>
      </div>
      <div class="desc-wrapper">
        <p class="tip">另需配送费用</p>
      </div>
    </div>
    <!-- 底部右侧 -->
    <div class="content-right">
      <div class="content-right">
        $0元起送
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.shopcart-wrapper{
  width: 100%;
  height: 51px;
  background: #514f4f;
  position: fixed;
  left: 0;
  bottom: 0;
  display: flex;
  z-index: 99;
}
.shopcart-wrapper .content-left{
  flex: 1;
}

.shopcart-wrapper .content-right{
  flex: 0 0 110px;
}
</style>
