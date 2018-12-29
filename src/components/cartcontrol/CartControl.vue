<template>
  <div class="cartcontrol">
    <div class="cart-decrease icon-remove_circle_outline"></div>
    <div class="cart-count">7</div>
    <div class="cart-add icon-add_circle">
      <i class="bg"></i>
    </div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>
@import url(../../common/css/icon.css);

.cartcontrol{
  font-size: 0;
}

.cartcontrol .cart-decrease{
  display: inline-block;
  width: 26px;
  height: 26px;
  font-size: 26px;
  color: #b4b4b4;
}

.cartcontrol .cart-add .bg{
  width: 20px;
  height: 20px;
  border-radius: 50%;
  background: black;
  position: absolute;
  left: 3px;
  top: 3px;
  z-index: -1;
}


.cartcontrol .cart-count{
  display: inline-block;
  width: 25px;
  text-align: center;
  font-size: 12px;
  line-height: 26px;
  vertical-align: top;
}

.cartcontrol .cart-add{
  display: inline-block;
  width: 26px;
  height: 26px;
  font-size: 26px;
  color: #ffd161;
  position: relative;
}

</style>
