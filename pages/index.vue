<template>
  <div class="container">
    <ZoomLoadingComponent />
    <SpinnerLoadingComponent />
    <SpinningLoadingComponent />
    <BouncingLoaderComponent />
  </div>
</template>

<script>
import ZoomLoadingComponent from "../components/zoom-loading.vue";
import SpinnerLoadingComponent from "../components/spinner-loading.vue";
import SpinningLoadingComponent from "../components/spinning-loading.vue";
import BouncingLoaderComponent from "../components/bouncing-loading.vue";

export default {
  name: "IndexPage",
  components: {
    ZoomLoadingComponent,
    SpinnerLoadingComponent,
    SpinningLoadingComponent,
    BouncingLoaderComponent,
  },
};
</script>

<style scoped>
.container {
  width: 100vw;
  height: 100vh;
  background-color: #180a0a;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
</style>
