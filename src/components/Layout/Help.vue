<template>
  <div class="main-help">
    <div class="help"></div>
    <slot name="help"></slot>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.main-help {
  background-color: transparent;
  background-image: linear-gradient(
    160deg,
    rgba(0, 117, 39, 0.07) 50%,
    #ffffff 50%
  );
  .help {
    background-color: transparent;
    background-image: radial-gradient(
      at center center,
      #a0e1d9 36%,
      rgba(0, 117, 39, 0.83) 100%
    );
    opacity: 0.05;
    transition: background 0.3s, border-radius 0.3s, opacity 0.3s;
  }
  .screen-center-min {
    max-width: 650px;
    margin: auto;
  }
  .custom-p {
    font-size: 20px;
  }
  .custom-h6 {
    font-size: 40px;
  }
  .vision-img {
    max-width: 450px!important;
    width: 100%;
  }
}
</style>
