<template>
  <div class="row screen-center about">
    <div class="col col-xs-12 col-sm-3 q-my-auto q-px-sm">
      <img src="@/assets/images/about/01.jpeg" alt="owner" />
    </div>
    <div class="col col-xs-12 col-sm-9 q-px-xl">
      <h6>
        GJ Allied company (Pvt.) ltd. has completed 10 years of its operations
        and today we are one of a leading construction company of the country.
        This has become possible only with untiring efforts of our dedicated
        staff and encouragement from our valued clients.
        <br />
        <br />
        GJ Allied was formed to deliver hassle free projects in timely and cost
        effective manners. We feel proud in telling that in the history of the
        company neither we have obtained any claim nor are we in litigation with
        any of our clients. We have positioned ourselves as such that we are
        ready to accept any construction challenge no matter how complex or huge
        it is. Since road to success is always under construction philosophy is
        that “WE CONSTRUCT RELIGIOUSLY”.
        <br />
        <br />
        I invite you to explore our website & get more information regarding GJ
        Allied.
        <br />
        <br />
        Malik Ghullam Jellani
        <br />
        <br />
        Chief Executive
      </h6>
    </div>
  </div>
  <Help>
    <template #help>
      <div class="screen-center text-center our-vision">
        <h5 class="q-py-md q-my-none custom-h6">
          OUR VISION
        </h5>
        <p class="q-my-xl custom-p text-left">
          At GJ allied, we mean to give exceptional enlistment administrations
          and answers for gain the best ability in the market. We will locate
          the most ideal possibility for your association. We viably evaluate
          and create aptitudes, keeping our partners on the ball, so they can
          take care of business each time, without fail.
        </p>
      </div>
      <div class="row justify-evenly screen-center our-vision">
        <div class="col col-xs-12 col-sm-6 text-center q-px-md">
          <div>
            <h5 class="text-left q-my-sm">
              The GJ Allied vision enhances the internal culture, and maintains
              GJ Allied reputation as a construction leader, an employer of
              choice, a trustworthy and respected contractor and an active
              community member. GJ Allied aspires to be the most respected
              builder, renowned for:<br /><br />
              <li>Excellence</li>
              <li>Leadership</li>
              <li>Unsurpassed value</li>
              <li>Quality</li>
              <li>Professionalism</li>
              <li>Corporate Social Responsibility</li>
            </h5>
          </div>
        </div>
        <div class="col col-xs-12 col-sm-6 text-center q-px-md q-my-auto">
          <img
            class="vision-img"
            src="@/assets/images/about/02.png"
            alt="icon-2"
          />
        </div>
      </div>
    </template>
  </Help>
  <div class="row screen-center justify-center our-mission">
    <h3 class="text-center">OUR MISSION</h3>
    <h6>
      Our main goal is to attempt ourselves as trusted and significant
      organization which endeavors to turn into the best Manpower supplier in
      Pakistan by reliably sending the best qualified staff while carefully
      clinging to rules set by the Government of Pakistan and offering need to
      the customer needs. We will keep on obtaining pertinent data and grow our
      insight and ability to guarantee this. GJ allied is to build on our
      reputation for integrity, excellence, experience, professionalism and
      leadership as the nation’s finest construction organization by strict
      adherence to our core values and by:
    </h6>
    <div class="col col-xs-12 col-sm-7">
      <h6>
        <li>Continuously improving the quality of our work and services.</li>
        <li>Constantly striving to exceed each client’s expectations.</li>
        <li>Maintaining our dedication to the highest moral principles.</li>
        <li>
          Providing our people with a challenging, secure and safe environment
          in which to achieve personal career goals.
        </li>
        <li>
          Contributing to the community by researching and developing new and
          more efficient and eco-friendly methods and solutions for our work and
          services.
        </li>
      </h6>
    </div>
    <div class="col col-xs-12 col-sm-5">
      <img
        class="allied-img"
        src="@/assets/images/about/03.jpeg"
        alt="Allied Services"
      />
    </div>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import Help from "../components/Layout/Help.vue";
export default defineComponent({
  components: {
    Help
  }
});
</script>

<style lang="scss">
.about {
  img {
    width: 100%;
  }
}
.our-mission {
  .allied-img {
    height: 450px;
  }
  li {
    margin: 10px 0;
  }
}
</style>
