<template>
  <div class="loader">
    <div class="bar"></div>
    <div class="bar"></div>
    <div class="bar"></div>
  </div>
</template>

<script>
export default {
  name: "ScaleLoadingAnimationComponent",
};
</script>

<style scoped>
.loader {
  display: flex;
  align-items: center;
}
.bar {
  display: inline-block;
  width: 3px;
  height: 40px;
  background-color: rgba(255, 255, 255, 0.5);
  border-radius: 10px;
  animation: scale-up 1s linear infinite;
}
.bar:nth-child(2) {
  height: 70px;
  margin: 0 10px;
  animation-delay: 0.25s;
}
.bar:nth-child(3) {
  animation-delay: 0.5s;
}
@keyframes scale-up {
  20% {
    background-color: #fff;
    transform: scaleY(1.5);
  }
  40% {
    transform: scaleY(1);
  }
}
</style>
