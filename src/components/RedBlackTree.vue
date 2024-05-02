<template>
  <div :class="$style.redBlackTree" :style="redBlackTreeStyle">
    <div :class="$style.heightBalancedTree">
      <h1 :class="$style.wakatobi">{{wakatobi}}</h1>
      <div :class="$style.sandAndSerenity" :style="sandAndSerenityStyle">
        {{sandAndSerenityAtWakatobi}}
      </div>
      <div :class="$style.button">
        <div :class="$style.open">Open</div>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";
  import type * as CSS from "csstype";

  export default defineComponent({
    name: "RedBlackTree",
    props: {
      wakatobi: { type: String },
      sandAndSerenityAtWakatobi: { type: String },
      propPadding: { type: [Object, Array, String, Number, Boolean] },
      propAlignSelf: { type: String },
    },
    computed: {
      redBlackTreeStyle(): CSS.Properties {
        return {
          padding: this.propPadding,
        };
      },
      sandAndSerenityStyle(): CSS.Properties {
        return {
          alignSelf: this.propAlignSelf,
        };
      },
    },
  });
</script>
<style module>
  .wakatobi {
    margin: 0;
    align-self: stretch;
    position: relative;
    font-size: inherit;
    line-height: 110%;
    font-weight: 600;
    font-family: inherit;
  }
  .sandAndSerenity {
    align-self: stretch;
    position: relative;
    font-size: var(--subheading-size);
    line-height: 150%;
    color: var(--color-gray);
  }
  .open {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 42px;
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
    font-size: var(--small-text-size);
    color: var(--color-white);
  }
  .heightBalancedTree {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xl);
  }
  .redBlackTree {
    width: 559px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-89xl) 0px 0px;
    box-sizing: border-box;
    min-width: 559px;
    max-width: 100%;
    text-align: left;
    font-size: var(--heading-size);
    color: var(--color-black);
    font-family: var(--small-text);
  }

  @media screen and (max-width: 2025px) {
    .wakatobi {
      font-size: var(--font-size-13xl);
      line-height: 35px;
    }

    .redBlackTree {
      flex: 1;
      min-width: 100%;
    }
  }
  @media screen and (max-width: 450px) {
    .wakatobi {
      font-size: var(--subheading-size);
      line-height: 26px;
    }

    .sandAndSerenity {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }
  }
</style>
