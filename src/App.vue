<template>
  <div id="app" class="app">
    <Header />
    <router-view />
  </div>
</template>
<script>
import Header from '@/components/Header';

export default {
  name: 'app',
  components: { Header }
};
</script>
<style lang="scss">
@import './styles/App.scss';
</style>
