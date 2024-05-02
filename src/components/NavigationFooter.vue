<template>
  <div :class="$style.navigationFooter">
    <div :class="$style.divider" />
    <div :class="$style.wingsParent">
      <b :class="$style.wings">WINGS</b>
      <div :class="$style.buttonsIconParent">
        <img
          :class="$style.buttonsIcon"
          loading="lazy"
          alt=""
          src="/buttons--icon@2x.png"
        />
        <img
          :class="$style.buttonsIcon1"
          loading="lazy"
          alt=""
          src="/buttons--icon-1@2x.png"
        />
        <img
          :class="$style.buttonsIcon2"
          loading="lazy"
          alt=""
          src="/buttons--icon-2@2x.png"
        />
        <img
          :class="$style.buttonsIcon3"
          loading="lazy"
          alt=""
          src="/buttons--icon-3@2x.png"
        />
      </div>
    </div>
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "NavigationFooter",
  });
</script>
<style module>
  .divider {
    width: 1281px;
    height: 1px;
    position: relative;
    border-top: 1px solid var(--color-gainsboro-100);
    box-sizing: border-box;
    max-width: 100%;
  }
  .wings {
    position: relative;
    line-height: 150%;
    display: inline-block;
    min-width: 84px;
  }
  .buttonsIcon {
    height: 40px;
    width: 40px;
    position: relative;
    border-radius: var(--br-9xs);
    object-fit: cover;
    min-height: 40px;
  }
  .buttonsIcon1 {
    height: 40px;
    width: 40px;
    position: relative;
    border-radius: var(--br-9xs);
    object-fit: cover;
    min-height: 40px;
  }
  .buttonsIcon2 {
    height: 40px;
    width: 40px;
    position: relative;
    border-radius: var(--br-9xs);
    object-fit: cover;
    min-height: 40px;
  }
  .buttonsIcon3 {
    height: 40px;
    width: 40px;
    position: relative;
    border-radius: var(--br-9xs);
    object-fit: cover;
    min-height: 40px;
  }
  .buttonsIconParent {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .wingsParent {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    gap: var(--gap-xl);
  }
  .navigationFooter {
    align-self: stretch;
    background-color: var(--color-rosybrown);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-12xs) var(--padding-7xl) var(--padding-10xl)
      var(--padding-61xl);
    box-sizing: border-box;
    gap: var(--gap-31xl);
    max-width: 100%;
    text-align: left;
    font-size: var(--subheading-size);
    color: var(--color-black);
    font-family: var(--small-text);
  }

  @media screen and (max-width: 2025px) {
    .navigationFooter {
      gap: var(--gap-6xl);
      padding-left: var(--padding-21xl);
      box-sizing: border-box;
    }
  }
  @media screen and (max-width: 450px) {
    .wings {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .wingsParent {
      flex-wrap: wrap;
    }
  }
</style>
