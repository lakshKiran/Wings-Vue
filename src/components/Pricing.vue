<template>
  <div :class="$style.pricing">
    <div :class="$style.navigation">
      <frame propWidth="245px" propGap="14px" />
      <div :class="$style.navigationInner">
        <div :class="$style.frameParent">
          <div :class="$style.articlesWrapper">
            <div :class="$style.articles">Articles</div>
          </div>
          <div :class="$style.frameWrapper">
            <div :class="$style.frameContainer">
              <div :class="$style.frameDiv">
                <div :class="$style.destinationsWrapper">
                  <div :class="$style.destinations">Destinations</div>
                </div>
              </div>
            </div>
          </div>
          <div :class="$style.hotelsWrapper">
            <div :class="$style.hotels">Hotels</div>
          </div>
          <div :class="$style.cruisesWrapper">
            <div :class="$style.cruises">Cruises</div>
          </div>
          <div :class="$style.button">
            <div :class="$style.signUp">Sign Up</div>
          </div>
        </div>
      </div>
    </div>
    <div :class="$style.dataGatherer">
      <div :class="$style.logicGateParent">
        <div :class="$style.logicGate">
          <div :class="$style.valueHolder">
            <h1 :class="$style.pricing1">Pricing</h1>
            <div :class="$style.longLastingConnectionsThriv">
              Long-lasting connections thrive on affordability as the
              cornerstone.
            </div>
          </div>
        </div>
        <div :class="$style.conditionChecker">
          <div :class="$style.pricingGrid">
            <Pricing1
              monthlyPlan="Monthly plan"
              errorHandler="$5"
              perMonth="per month"
            /><Pricing1
              monthlyPlan="Annual plan"
              errorHandler="$50"
              perMonth="per year"
              propMinWidth="90px"
              propMinWidth1="78px"
              propMinWidth2="64px"
            />
          </div>
        </div>
        <div :class="$style.dataSampler">
          <h1 :class="$style.frequentlyAskedQuestions">
            Frequently Asked Questions
          </h1>
          <div :class="$style.dataFilter">
            <div :class="$style.dataCompressor">
              <div :class="$style.dataExpander">
                <div :class="$style.canUsersSet">
                  Can users set preferences on the types of articles for them to
                  be notified
                </div>
                <div :class="$style.wingsProvidesOptions">
                  Wings provides options to set preferences based on locations,
                  destination types, among other attributes
                </div>
              </div>
            </div>
            <h1 :class="$style.dataSplitter">+</h1>
          </div>
          <div :class="$style.dataSink">
            <div :class="$style.dataStream">
              <div :class="$style.whatIsWings">
                What is wings cancellation policy ?
              </div>
            </div>
            <h1 :class="$style.dataPool">+</h1>
          </div>
          <div :class="$style.dataSink1">
            <div :class="$style.doesWingsProvidePersonalizeWrapper">
              <div :class="$style.doesWingsProvide">
                Does Wings provide personalized dashboard ?
              </div>
            </div>
            <h1 :class="$style.h1">+</h1>
          </div>
        </div>
      </div>
    </div>
    <NavigationFooter />
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";
  import Frame from "./Frame.vue";
  import Pricing1 from "./Pricing1.vue";
  import NavigationFooter from "./NavigationFooter.vue";

  export default defineComponent({
    name: "Pricing",
    components: { Frame, Pricing1, NavigationFooter },
  });
</script>
<style module>
  .articles {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 74px;
  }
  .articlesWrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-2xs) 0px 0px;
  }
  .destinations {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 120px;
  }
  .destinationsWrapper {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
  }
  .frameDiv {
    background-color: var(--color-rosybrown);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
  }
  .frameContainer {
    background-color: var(--color-rosybrown);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: var(--padding-3xs);
    z-index: 1;
  }
  .frameWrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-12xs) var(--padding-3xs) 0px 0px;
  }
  .hotels {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 62px;
    z-index: 1;
  }
  .hotelsWrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-2xs) var(--padding-lg) 0px 0px;
  }
  .cruises {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 73px;
  }
  .cruisesWrapper {
    width: 104px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-2xs) var(--padding-xl) 0px 0px;
    box-sizing: border-box;
  }
  .signUp {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 60px;
  }
  .button {
    box-shadow: var(--button-shadow);
    border-radius: var(--br-5xs);
    background-color: var(--color-black);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-sm) var(--padding-5xl);
    white-space: nowrap;
    font-size: var(--small-text-size);
    color: var(--color-rosybrown);
  }
  .frameParent {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-mid);
  }
  .navigationInner {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-10xl) 0px 0px;
    box-sizing: border-box;
    max-width: 100%;
  }
  .navigation {
    align-self: stretch;
    background-color: var(--color-rosybrown);
    overflow: hidden;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    padding: var(--padding-8xl) var(--padding-61xl) var(--padding-8xl)
      var(--padding-3xs);
    box-sizing: border-box;
    max-width: 100%;
    gap: var(--gap-xl);
  }
  .pricing1 {
    margin: 0;
    align-self: stretch;
    position: relative;
    font-size: inherit;
    letter-spacing: -0.02em;
    font-weight: 700;
    font-family: inherit;
  }
  .longLastingConnectionsThriv {
    align-self: stretch;
    position: relative;
    font-size: var(--subheading-size);
    line-height: 150%;
    color: var(--color-gray);
  }
  .valueHolder {
    width: 912.8px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xl);
    max-width: 100%;
  }
  .logicGate {
    width: 1119px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl) var(--padding-4xs);
    box-sizing: border-box;
    max-width: 100%;
    text-align: center;
  }
  .pricingGrid {
    width: 842px;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-11xs) 0px 0px;
    box-sizing: border-box;
    gap: 32px 30px;
    max-width: 100%;
  }
  .conditionChecker {
    width: 1102px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl);
    box-sizing: border-box;
    max-width: 100%;
    font-size: var(--small-text-size);
  }
  .frequentlyAskedQuestions {
    margin: 0;
    align-self: stretch;
    position: relative;
    font-size: var(--heading-size);
    line-height: 110%;
    font-weight: 600;
    font-family: inherit;
  }
  .canUsersSet {
    align-self: stretch;
    position: relative;
    line-height: 150%;
  }
  .wingsProvidesOptions {
    width: 956px;
    position: relative;
    font-size: var(--body-text-size);
    line-height: 150%;
    font-weight: 500;
    color: var(--color-gray);
    display: flex;
    align-items: center;
    max-width: 100%;
  }
  .dataExpander {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-17xl);
    max-width: 100%;
  }
  .dataCompressor {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-9xs) 0px 0px;
    box-sizing: border-box;
    min-width: 785px;
    max-width: 100%;
  }
  .dataSplitter {
    margin: 0;
    width: 27px;
    position: relative;
    font-size: var(--heading-size);
    line-height: 110%;
    font-weight: 600;
    font-family: inherit;
    color: var(--color-gray);
    display: inline-block;
  }
  .dataFilter {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xl);
    max-width: 100%;
  }
  .whatIsWings {
    align-self: stretch;
    position: relative;
    line-height: 150%;
  }
  .dataStream {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-9xs) 0px 0px;
    box-sizing: border-box;
    min-width: 785px;
    max-width: 100%;
  }
  .dataPool {
    margin: 0;
    width: 27px;
    position: relative;
    font-size: var(--heading-size);
    line-height: 110%;
    font-weight: 600;
    font-family: inherit;
    color: var(--color-gray);
    display: inline-block;
  }
  .dataSink {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xl);
    max-width: 100%;
  }
  .doesWingsProvide {
    align-self: stretch;
    position: relative;
    line-height: 150%;
  }
  .doesWingsProvidePersonalizeWrapper {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-9xs) 0px 0px;
    box-sizing: border-box;
    min-width: 785px;
    max-width: 100%;
  }
  .h1 {
    margin: 0;
    width: 27px;
    position: relative;
    font-size: var(--heading-size);
    line-height: 110%;
    font-weight: 600;
    font-family: inherit;
    color: var(--color-gray);
    display: inline-block;
  }
  .dataSink1 {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xl);
    max-width: 100%;
  }
  .dataSampler {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-13xl);
    max-width: 100%;
    font-size: var(--subheading-size);
  }
  .logicGateParent {
    width: 1259px;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: flex-start;
    gap: var(--gap-73xl);
    max-width: 100%;
  }
  .dataGatherer {
    width: 1421px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl) var(--padding-132xl);
    box-sizing: border-box;
    max-width: 100%;
    flex-shrink: 0;
    font-size: var(--title-size);
  }
  .pricing {
    align-self: stretch;
    height: 1773px;
    background-color: var(--color-gainsboro-400);
    overflow: hidden;
    flex-shrink: 0;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-12xs) var(--padding-332xl) 0px;
    box-sizing: border-box;
    gap: var(--gap-61xl);
    max-width: 100%;
    text-align: left;
    font-size: var(--body-text-size);
    color: var(--color-black);
    font-family: var(--small-text);
  }

  @media screen and (max-width: 2025px) {
    .frameParent {
      flex-wrap: wrap;
    }

    .navigation {
      flex-wrap: wrap;
      padding-right: var(--padding-21xl);
      box-sizing: border-box;
    }

    .pricing1 {
      font-size: var(--font-size-32xl);
    }

    .frequentlyAskedQuestions {
      font-size: var(--font-size-13xl);
      line-height: 35px;
    }

    .dataExpander {
      gap: var(--gap-lg);
    }

    .dataCompressor {
      min-width: 100%;
    }

    .dataSplitter {
      font-size: var(--font-size-13xl);
      line-height: 35px;
    }

    .dataFilter {
      flex-wrap: wrap;
    }

    .dataStream {
      min-width: 100%;
    }

    .dataPool {
      font-size: var(--font-size-13xl);
      line-height: 35px;
    }

    .dataSink {
      flex-wrap: wrap;
    }

    .doesWingsProvidePersonalizeWrapper {
      min-width: 100%;
    }

    .h1 {
      font-size: var(--font-size-13xl);
      line-height: 35px;
    }

    .dataSink1 {
      flex-wrap: wrap;
    }

    .dataSampler {
      gap: var(--gap-base);
    }

    .logicGateParent {
      gap: var(--gap-27xl);
    }

    .dataGatherer {
      padding-bottom: var(--padding-45xl);
      box-sizing: border-box;
    }

    .pricing {
      height: auto;
      gap: var(--gap-21xl);
      padding-bottom: var(--padding-77xl);
      box-sizing: border-box;
    }
  }
  @media screen and (max-width: 450px) {
    .articles {
      font-size: var(--small-text-size);
      line-height: 24px;
    }

    .destinations {
      font-size: var(--small-text-size);
      line-height: 24px;
    }

    .hotels {
      font-size: var(--small-text-size);
      line-height: 24px;
    }

    .cruises {
      font-size: var(--small-text-size);
      line-height: 24px;
    }

    .pricing1 {
      font-size: var(--font-size-19xl);
    }

    .longLastingConnectionsThriv {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .frequentlyAskedQuestions {
      font-size: var(--subheading-size);
      line-height: 26px;
    }

    .canUsersSet {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .wingsProvidesOptions {
      font-size: var(--small-text-size);
      line-height: 24px;
    }

    .dataSplitter {
      font-size: var(--subheading-size);
      line-height: 26px;
    }

    .whatIsWings {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .dataPool {
      font-size: var(--subheading-size);
      line-height: 26px;
    }

    .doesWingsProvide {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .h1 {
      font-size: var(--subheading-size);
      line-height: 26px;
    }

    .logicGateParent {
      gap: var(--gap-4xl);
    }

    .pricing {
      gap: var(--gap-xl);
    }
  }
</style>
