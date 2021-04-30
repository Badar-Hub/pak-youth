<template>
  <div class="footer q-py-xl q-mt-xl">
    <div class="row sub-footer screen-center">
      <div :class="!$q.screen.gt.xs ? 'text-center' : ''" class="col col-xs-12 col-sm-6 q-my-auto">
        <div class="logo">
          <img src="@/assets/logo.png" alt="logo" />
        </div>
        <h4>Gj Allied Services Pvt Ltd</h4>
      </div>
      <div class="col col-xs-12 col-sm-6 q-my-auto q-px-md">
        <img class="map" src="@/assets/images/map.png" alt="map" />
      </div>
      <div class="col-12">
        <div :class="!$q.screen.gt.xs ? 'justify-center' : ''" class="row">
          <q-icon name="facebook" size="xl" />
          <q-icon name="fab fa-twitter" size="xl" />
        </div>
      <p :class="!$q.screen.gt.xs ? 'text-center' : ''" class="q-my-none">Copyright © 2021 Tech Origin</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
};
</script>

<style lang="scss">
.footer {
  width: 100%;
  background-image: url("../../assets/images/footer.png");
  max-height: 4500px;
  height: auto;
  background-color: #333333;
  color: white;
  .sub-footer {
    height: 100%;
  }
  .map {
    width: 100%;
  }
  .logo {
    img {
      max-width: 150px;
      &:hover {
        max-width: 180px;
      }
    }
  }
}
</style>
