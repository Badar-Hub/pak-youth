<template>
  <div class="home">
    <Slider />
    <div class="bg-img text-center">
      <div class="row screen-center q-my-md">
        <div class="col col-xs-12 col-sm-6">
          <h6 class="q-my-sm">OUR EXPERTISE</h6>
          <p class="q-my-sm">
            GJ Allied has diversified experience of multi storey building,
            infrastructure, interior designing, value engineering and project
            management. In over 10 years of experience we have been building
            life time relationships with our clients through our services under
            supervisions of professionals.
          </p>
        </div>
        <div class="col col-xs-12 col-sm-6 q-px-xl">
          <q-linear-progress size="25px" :value="progress1" color="#007527">
            <div class="absolute-full flex flex-center">
              <q-badge
                color="white"
                text-color="accent"
                :label="progressLabel1"
              />
            </div>
          </q-linear-progress>
          <q-linear-progress size="25px" :value="progress1" color="#007527">
            <div class="absolute-full flex flex-center">
              <q-badge
                color="white"
                text-color="accent"
                :label="progressLabel1"
              />
            </div>
          </q-linear-progress>
          <q-linear-progress size="25px" :value="progress1" color="#007527">
            <div class="absolute-full flex flex-center">
              <q-badge
                color="white"
                text-color="accent"
                :label="progressLabel1"
              />
            </div>
          </q-linear-progress>
          <q-linear-progress size="25px" :value="progress1" color="#007527">
            <div class="absolute-full flex flex-center">
              <q-badge
                color="white"
                text-color="accent"
                :label="progressLabel1"
              />
            </div>
          </q-linear-progress>
        </div>
      </div>
    </div>
    <OurClients />
    <Help>
      <template #help>
        <div class="screen-center-min text-center q-py-lg">
          <h6 class="q-py-md q-my-none custom-h6">
            How May I Help You?
          </h6>
          <p class="q-my-xl custom-p">
            GJ Allied has diversified experience of multi storey building,
            infrastructure, interior designing, value engineering and project
            management. In over 10 years of experience we have been building
            life time relationships with our clients through our services under
            supervisions of professionals.
          </p>
        </div>
        <div class="row justify-evenly screen-center q-my-xl">
          <div class="col col-xs-12 col-sm-4 text-center q-px-md">
            <img src="@/assets/images/icon/01.png" alt="icon-1" />
            <p>
              GJ Allied have opened doors for many clients to find their desired
              property and make the right investment at the right time. We deal
              in all types of residential and commercial properties at a
              reasonable price.
            </p>
          </div>
          <div class="col col-xs-12 col-sm-4 text-center q-px-md">
            <img src="@/assets/images/icon/02.png" alt="icon-2" />
            <p>
              GJ Allied provide Multi-Skilling engineers, labour in Construction
              Industry in Pakistan
            </p>
          </div>
          <div class="col col-xs-12 col-sm-4 text-center q-px-md">
            <img src="@/assets/images/icon/03.png" alt="icon-3" />
            <p>
              GJ Allied provide for the safety & health of all personnel
              involved in the Project and the safe operation of the completed
              facilities to achieve zero lost-time incidents.
            </p>
          </div>
        </div>
        <div class="row screen-center justify-center q-my-md">
          <q-btn color="green" label="View More" />
        </div>
      </template>
    </Help>
    <div class="row screen-center justify-center">
      <h3 class="text-center">WHY CHOOSE US</h3>
      <img class="chose-us" src="@/assets/images/03.png" alt="why-chose-us" />
    </div>
    <div class="row justify-center">
      <iframe
        width="1200"
        height="721"
        src="https://www.youtube.com/embed/m3EG8n0Vu6s"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref, computed } from "vue";
import Slider from "../components/Layout/Slider.vue";
import OurClients from "../components/Layout/OurClients";
import Help from "../components/Layout/Help";
export default defineComponent({
  components: {
    Slider,
    OurClients,
    Help
  },
  setup() {
    const progress1 = ref(0.9);

    return {
      progress1,
      progressLabel1: computed(() => (progress1.value * 100).toFixed(2) + "%")
    };
  }
});
</script>

<style lang="scss">
.home {
  .bg-img {
    background-image: url("../assets/images/02.jpeg");
    background-repeat: no-repeat;
    background-size: cover;
  }
  h6 {
    font-size: 30px;
    color: black;
  }
  p {
    color: #3a3a3a;
    font-size: 16px;
    font-weight: 700;
  }
  .q-linear-progress {
    border-radius: 10%;
    margin: 10px 0;
  }
  .chose-us {
    width: 100%;
  }
}
</style>
