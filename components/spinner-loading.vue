<template>
  <div class="spinner-loading-wrapper">
    <div class="spinner-loading">
      <div class="spinner-loading spinner-loading-linear"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SpinnerLoadingComponent",
};
</script>

<style scoped>
.spinner-loading-wrapper {
  width: 140px;
  height: 140px;
}

.spinner-loading {
  box-sizing: border-box;
  width: 100%;
  height: 100%;
  border: 10px solid transparent;
  border-top-color: #4bc8eb;
  border-bottom-color: #f13a8f;
  border-radius: 50%;
  animation: rotate 5s linear infinite;
}

.spinner-loading-linear {
  border-top-color: #36f372;
  border-bottom-color: #fff;
  animation-duration: 2.5s;
}

@keyframes rotate {
  0% {
    transform: scale(1) rotate(360deg);
  }
  50% {
    transform: scale(0.8) rotate(-360deg);
  }
  100% {
    transform: scale(1) rotate(360deg);
  }
}
</style>
