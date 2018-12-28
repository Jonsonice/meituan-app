<template>
  <div id="app">
    <!-- 头部 -->
    <app-header :poiInfo="poiInfo"></app-header>
    
    <!-- 导航 -->
    <div class="nav">
      <app-nav></app-nav>
    </div>
    
    <!-- 内容 -->
    <router-view></router-view>
  </div>
</template>

<script>
import Header from './components/header/Header';
import Nav from './components/nav/Nav';

export default {
    name: 'App',
    data() {
        return {
            poiInfo: {}
        };
    },
    components: {
        'app-header': Header,
        'app-nav': Nav
    },
    created() {
        fetch('/api/goods')
            .then(res => {
                return res.json();
            })
            .then(response => {
                // console.log(response)
                if (response.code == 0) {
                    this.poiInfo = response.data.poi_info;
                    // console.log(this.poiInfo);
                }
            });
    }
};
</script>

<style>
</style>
