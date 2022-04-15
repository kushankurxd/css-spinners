<template>
  <div class="spinner"></div>
</template>

<script>
export default {
  name: "SpinningLoadingComponent",
};
</script>

<style scoped>
.spinner {
  position: relative;
  width: 100px;
  height: 100px;
  border-radius: 50%;
}
.spinner::before,
.spinner:after {
  content: "";
  position: absolute;
  border-radius: inherit;
}
.spinner:before {
  width: 100%;
  height: 100%;
  background-image: linear-gradient(0deg, #ff00cc 0%, #333399 100%);
  animation: spin 0.5s infinite linear;
}
.spinner:after {
  width: 85%;
  height: 85%;
  background-color: #180a0a;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
@keyframes spin {
  to {
    transform: rotate(360deg);
  }
}
</style>
