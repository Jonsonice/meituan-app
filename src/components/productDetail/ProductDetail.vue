<template>
  <transition name="food-detail">
    <div class="food" v-show="showFlag">
      <div class="food-wrapper">
        <div class="food-content">
          <div class="img-wrapper">
            <img class="food-img" />
            <span 
              class="close-bt icon-close"
              @click="closeView"></span>
            <img class="share-bt" src="./img/share.png" />
            <img class="more-bt" src="./img/more.png" />
          </div>

          <div class="content-wrapper">
            <h3 class="name"></h3>
              <p class="saled"></p>
              <img class="product">
              <p class="price">
                <span class="text"></span>
                <span class="unit"></span>
              </p>

              <div class="cartcontrol-wrapper">
                <CartControl :food="food"></CartControl>
              </div>
              <div 
                class="buy" 
                >
                选规格
              </div>
          </div>
        </div>
      </div>
    </div>
  </transition>
</template>

<script>
  import CartControl from '../cartcontrol/CartControl'
  export default {
    data(){
      return {
        showFlag:false
      }
    },
    props:{
      food:{
        type:Object
      }
    },
    methods:{
      showView(){
        this.showFlag = true
      },
      closeView(){
        this.showFlag = false
      },
    },
    components:{
      CartControl
    }
  }
</script>

<style scoped>
@import url(../../common/css/icon.css);

.food{
  position: fixed;
  left: 0;
  top: 0;
  bottom: 51px;
  background: white;
  width: 100%;
  z-index: 90;
}
</style>
