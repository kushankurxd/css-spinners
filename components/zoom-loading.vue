<template>
  <div class="loader"></div>
</template>

<script>
export default {
  name: "ZoomLoadingComponent",
};
</script>

<style scoped>
.loader {
  width: 100px;
  height: 100px;
  position: relative;
  z-index: 0;
}
.loader::before,
.loader::after {
  content: "";
  position: absolute;
  width: inherit;
  height: inherit;
  border-radius: 50%;
  mix-blend-mode: multiply;
  animation: rotate 1s infinite cubic-bezier(0.77, 0, 0.175, 1);
}
.loader::before {
  background-color: #fc3f9e;
}
.loader::after {
  background-color: #50e8f3;
  animation-delay: 0.5s;
}
@keyframes rotate {
  0%,
  100% {
    left: 95px;
  }
  25% {
    transform: scale(0.3);
  }
  50% {
    left: 0;
  }
  75% {
    transform: scale(1);
  }
}
</style>
