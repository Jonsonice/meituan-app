<template>
  <div id="app">
    <!-- 头部 -->
    <app-header></app-header>
    
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
    components: {
        'app-header': Header,
        'app-nav': Nav
    }
};
</script>

<style>
</style>
