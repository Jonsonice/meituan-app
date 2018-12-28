<template>
  <div class="nav">
   <router-link class="nav-item" to="/goods">
      点餐
    </router-link>
    <router-link class="nav-item" to="/ratings">
      评价
    </router-link>
    <router-link class="nav-item" to="/seller">
      商家
    </router-link>
  </div>
</template>

<script>
export default {}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.nav {
    display: flex;
    width: 100%;
    height: 40px;
    line-height: 40px;
    border-bottom: 1px solid #e4e4e4;
}
.nav-item {
    flex: 1;
    text-align: center;
    font-size: 13px;
    text-decoration: none;
    color: #666;
    position: relative;
}

</style>
