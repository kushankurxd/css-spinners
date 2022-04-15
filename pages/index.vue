<template>
  <div class="container">
    <ZoomLoadingComponent />
  </div>
</template>

<script>
import ZoomLoadingComponent from "../components/zoom-loading.vue";

export default {
  name: "IndexPage",
  components: {
    ZoomLoadingComponent,
  },
};
</script>

<style scoped>
.container {
  width: 100vw;
  height: 100vh;
  background-color: #000;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
