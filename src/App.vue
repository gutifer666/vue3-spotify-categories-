<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <Suspense>
    <template #default>
      <show-category />
    </template>
    <template #fallback>
      <span>Cargando...</span>
    </template>
  </Suspense>
</template>

<script>
import ShowCategory from "./components/ShowCategory.vue";
export default {
  name: "App",
  components: {
    ShowCategory,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>