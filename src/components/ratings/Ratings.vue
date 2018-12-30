<template>
  <div class="ratings">
	 <div class="ratings-wrapper">
      <div class="overview">
        <div class="overview-left">
          <div class="comment-score">
            <p class="score"></p>
            <p class="text">商家评分</p>
          </div>
          <div class="other-score">
            <div class="quality-score item">
              <span class="text">口味</span>
              <Star class='star'></Star>
              <span class="score"></span>
            </div>
            <div class="pack-score item">
              <span class="text">包装</span>
              <Star class='star'></Star>
              <span class="score"></span>
            </div>
          </div>
        </div>
      </div>
      <div class="overview-right">
        
      </div>
    </div>
    <Split></Split>

    <div class="content">

    </div>
  </div>
</template>

<script>
  import Split from '../split/Split'
  import Star from '../star/Star'

  export default {
    components:{
      Split,
      Star
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
