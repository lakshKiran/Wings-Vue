<template>
  <div :class="$style.pricing">
    <div :class="$style.ruleSet">
      <div :class="$style.monthlyPlan" :style="monthlyPlanStyle">
        {{monthlyPlan}}
      </div>
    </div>
    <div :class="$style.header">
      <div :class="$style.price">
        <div :class="$style.errorHandler" :style="errorHandlerStyle">
          {{errorHandler}}
        </div>
        <div :class="$style.perMonth" :style="perMonthStyle">{{perMonth}}</div>
      </div>
    </div>
    <div :class="$style.featureList">
      <div :class="$style.articles">
        <ul :class="$style.articles1">
          <li>Articles</li>
        </ul>
      </div>
      <div :class="$style.destinations">
        <ul :class="$style.destinations1">
          <li>Destinations</li>
        </ul>
      </div>
      <div :class="$style.hotels">
        <ul :class="$style.hotels1">
          <li>Hotels</li>
        </ul>
      </div>
      <div :class="$style.cruises">
        <ul :class="$style.cruises1">
          <li>Cruises</li>
        </ul>
      </div>
    </div>
    <div :class="$style.button">
      <div :class="$style.select">Select</div>
    </div>
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";
  import type * as CSS from "csstype";

  export default defineComponent({
    name: "Pricing1",
    props: {
      monthlyPlan: { type: String },
      errorHandler: { type: String },
      perMonth: { type: String },
      propMinWidth: { type: [Object, Array, String, Number, Boolean] },
      propMinWidth1: { type: [Object, Array, String, Number, Boolean] },
      propMinWidth2: { type: [Object, Array, String, Number, Boolean] },
    },
    computed: {
      monthlyPlanStyle(): CSS.Properties {
        return {
          minWidth: this.propMinWidth,
        };
      },
      errorHandlerStyle(): CSS.Properties {
        return {
          minWidth: this.propMinWidth1,
        };
      },
      perMonthStyle(): CSS.Properties {
        return {
          minWidth: this.propMinWidth2,
        };
      },
    },
  });
</script>
<style module>
  .monthlyPlan {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 100px;
  }
  .ruleSet {
    border-radius: var(--br-5xs);
    background-color: var(--color-gainsboro-200);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: var(--padding-5xs) var(--padding-base);
    white-space: nowrap;
  }
  .errorHandler {
    position: relative;
    line-height: 110%;
    font-weight: 600;
    display: inline-block;
    min-width: 52px;
    white-space: nowrap;
  }
  .perMonth {
    position: relative;
    font-size: var(--small-text-size);
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 79px;
  }
  .price {
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .header {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-end;
    font-size: var(--heading-size);
  }
  .articles1 {
    margin: 0;
    font-family: inherit;
    font-size: inherit;
    padding-left: var(--padding-8xl);
  }
  .articles {
    align-self: stretch;
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .destinations1 {
    margin: 0;
    font-family: inherit;
    font-size: inherit;
    padding-left: var(--padding-8xl);
  }
  .destinations {
    align-self: stretch;
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .hotels1 {
    margin: 0;
    font-family: inherit;
    font-size: inherit;
    padding-left: var(--padding-8xl);
  }
  .hotels {
    align-self: stretch;
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .cruises1 {
    margin: 0;
    font-family: inherit;
    font-size: inherit;
    padding-left: var(--padding-8xl);
  }
  .cruises {
    align-self: stretch;
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .featureList {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-end;
    gap: var(--gap-xs);
    font-size: var(--body-text-size);
    color: var(--color-gray);
  }
  .select {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 49px;
  }
  .button {
    align-self: stretch;
    box-shadow: var(--button-shadow);
    border-radius: var(--br-5xs);
    background-color: var(--color-black);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: var(--padding-sm) var(--padding-xl);
    color: var(--color-rosybrown);
  }
  .pricing {
    flex: 1;
    box-shadow: 0px 4px 6px -4px rgba(0, 0, 0, 0.1),
      0px 0px 15px rgba(0, 0, 0, 0.1);
    border-radius: var(--br-xs);
    background-color: var(--color-rosybrown);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-end;
    padding: var(--spacing-m);
    box-sizing: border-box;
    gap: var(--spacing-sm);
    min-width: 162px;
    max-width: 100%;
    text-align: left;
    font-size: var(--small-text-size);
    color: var(--color-black);
    font-family: var(--small-text);
  }

  @media screen and (max-width: 2025px) {
    .errorHandler {
      font-size: var(--font-size-13xl);
      line-height: 35px;
    }

    .pricing {
      padding-top: var(--spacing-m);
      padding-bottom: var(--spacing-m);
      box-sizing: border-box;
    }
  }
  @media screen and (max-width: 450px) {
    .errorHandler {
      font-size: var(--subheading-size);
      line-height: 26px;
    }

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

    .pricing {
      gap: var(--spacing-sm);
      padding-left: var(--spacing-m);
      padding-right: var(--spacing-m);
      box-sizing: border-box;
    }
  }
</style>
