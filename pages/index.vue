<template>
  <div class="container">
    <div class="sub-container">
      <SpinnerLoadingComponent />
      <SpinningLoadingComponent />
      <BouncingLoaderComponent />
    </div>
    <div class="sub-container">
      <ScaleLoadingAnimationComponent />
      <ZoomLoadingComponent />
    </div>
    <div class="sub-container">
      <BasketballLoadingComponent />
    </div>
  </div>
</template>

<script>
import ZoomLoadingComponent from "../components/zoom-loading.vue";
import SpinnerLoadingComponent from "../components/spinner-loading.vue";
import SpinningLoadingComponent from "../components/spinning-loading.vue";
import BouncingLoaderComponent from "../components/bouncing-loading.vue";
import BasketballLoadingComponent from "../components/basketball-loading.vue";
import ScaleLoadingAnimationComponent from "../components/scale-loading.vue";

export default {
  name: "IndexPage",
  components: {
    ZoomLoadingComponent,
    SpinnerLoadingComponent,
    SpinningLoadingComponent,
    BouncingLoaderComponent,
    BasketballLoadingComponent,
    ScaleLoadingAnimationComponent,
  },
};
</script>

<style scoped>
.container {
  width: 100vw;
  height: 100vh;
  background-color: #180a0a;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.sub-container {
  width: inherit;
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin: 4vh 0;
}
</style>
