<template>
  <div class="container">
    <ZoomLoadingComponent />
    <SpinnerLoadingComponent />
  </div>
</template>

<script>
import ZoomLoadingComponent from "../components/zoom-loading.vue";
import SpinnerLoadingComponent from "../components/spinner-loading.vue";

export default {
  name: "IndexPage",
  components: {
    ZoomLoadingComponent,
    SpinnerLoadingComponent,
  },
};
</script>

<style scoped>
.container {
  width: 100vw;
  height: 100vh;
  background-color: #180a0a;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
