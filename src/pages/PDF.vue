<template>
  <div :class="$style.pdf">
    <div :class="$style.landingPageWrapper"><LandingPage /></div>
    <div :class="$style.pricingWrapper"><Pricing /></div>
    <div :class="$style.dataSender"><ContactUs /></div>
    <Auth />
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";
  import LandingPage from "../components/LandingPage.vue";
  import Pricing from "../components/Pricing.vue";
  import ContactUs from "../components/ContactUs.vue";
  import Auth from "../components/Auth.vue";

  export default defineComponent({
    name: "PDF",
    components: { LandingPage, Pricing, ContactUs, Auth },
  });
</script>
<style module>
  .landingPageWrapper {
    width: 1560px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-5xs) 0px 0px;
    box-sizing: border-box;
    max-width: 100%;
  }
  .pricingWrapper {
    width: 1577px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-5xs) var(--padding-base) 0px 0px;
    box-sizing: border-box;
    max-width: 100%;
  }
  .dataSender {
    width: 1576px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-5xs) var(--padding-base) 0px 0px;
    box-sizing: border-box;
    max-width: 100%;
  }
  .pdf {
    width: 100%;
    position: relative;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    padding: 129px 49px 1557px 73px;
    box-sizing: border-box;
    line-height: normal;
    letter-spacing: normal;
    gap: var(--gap-xl);
  }

  @media screen and (max-width: 5250px) {
    .pdf {
      flex-wrap: wrap;
      justify-content: center;
    }
  }
  @media screen and (max-width: 3675px) {
    .pdf {
      flex-wrap: wrap;
      justify-content: center;
    }
  }
  @media screen and (max-width: 2025px) {
    .pdf {
      flex-wrap: wrap;
      justify-content: center;
      padding-left: 36px;
      padding-right: var(--padding-5xl);
      box-sizing: border-box;
    }
  }
  @media screen and (max-width: 450px) {
    .pdf {
      flex-wrap: wrap;
      justify-content: center;
    }
  }
</style>
