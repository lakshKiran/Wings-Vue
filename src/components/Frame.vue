<template>
  <div :class="$style.wings1Parent" :style="frameDivStyle">
    <img :class="$style.wings1Icon" loading="lazy" alt="" src="/wings-1.svg" />
    <div :class="$style.wingsWrapper">
      <h2 :class="$style.wings">WINGS</h2>
    </div>
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";
  import type * as CSS from "csstype";

  export default defineComponent({
    name: "Frame",
    props: {
      propWidth: { type: [Object, Array, String, Number, Boolean] },
      propGap: { type: String },
    },
    computed: {
      frameDivStyle(): CSS.Properties {
        return {
          width: this.propWidth,
          gap: this.propGap,
        };
      },
    },
  });
</script>
<style module>
  .wings1Icon {
    height: 110px;
    width: 109px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .wings {
    margin: 0;
    align-self: stretch;
    position: relative;
    font-size: inherit;
    line-height: 150%;
    font-weight: 500;
    font-family: inherit;
    text-shadow: 1px 0 0 #000, 0 1px 0 #000, -1px 0 0 #000, 0 -1px 0 #000;
    z-index: 1;
  }
  .wingsWrapper {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-10xl) 0px 0px;
  }
  .wings1Parent {
    width: 232px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-12xs);
    text-align: left;
    font-size: var(--font-size-13xl);
    color: var(--color-black);
    font-family: var(--small-text);
  }

  @media screen and (max-width: 2025px) {
    .wings {
      font-size: var(--font-size-7xl);
      line-height: 38px;
    }
  }
  @media screen and (max-width: 450px) {
    .wings {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }
  }
</style>
