<template>
  <div id="app">
<header>

  <hnav></hnav><!-- グローバルナビ -->
</header>
    <router-view/>
  </div>
</template>

<script>
import HeaderNav from '@/components/parts/NavHeader'
export default {
  name: 'App',
  components: {
    hnav: HeaderNav    
    }
}

</script>

<style>
#app {
font-family: 'Sawarabi Gothic', sans-serif;  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 20px;
}
</style>
