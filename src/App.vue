<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppSalesMenu from './components/AppSalesMenu.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppSalesMenu,
  }
}
</script>

<template>
  <div>
    <AppHeader />

    <AppMain />

    <AppSalesMenu />

    <AppFooter />
  </div>
</template>

<style lang="scss">
  @use './style/general.scss';
</style>