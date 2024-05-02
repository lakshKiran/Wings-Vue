<template>
  <div :class="$style.auth">
    <div :class="$style.linkCollection">
      <div :class="$style.navigation">
        <img
          :class="$style.wings1Icon"
          loading="lazy"
          alt=""
          src="/wings-1.svg"
        />
        <div :class="$style.symbolSwapper">
          <h2 :class="$style.wings">WINGS</h2>
        </div>
        <div :class="$style.tableSizeAdjuster">
          <div :class="$style.articles">Articles</div>
        </div>
        <div :class="$style.pathBender">
          <div :class="$style.symbolMergerWrapper">
            <div :class="$style.symbolMerger">
              <div :class="$style.destinationsWrapper">
                <div :class="$style.destinations">Destinations</div>
              </div>
            </div>
          </div>
        </div>
        <div :class="$style.shapeColorPicker">
          <div :class="$style.hotels">Hotels</div>
        </div>
        <div :class="$style.tableSizeAdjuster1">
          <div :class="$style.cruises">Cruises</div>
        </div>
        <div :class="$style.italicController">
          <div :class="$style.button">
            <div :class="$style.signUp">Sign Up</div>
          </div>
        </div>
      </div>
    </div>
    <div :class="$style.logicGate">
      <div :class="$style.createAnAccount">Create an account</div>
    </div>
    <div :class="$style.inputFilter">
      <div :class="$style.enterYourEmail">
        Enter your email to sign up for this app
      </div>
    </div>
    <div :class="$style.tableStyle">
      <div :class="$style.field">
        <div :class="$style.label">email@figmasfakedomain.net</div>
      </div>
    </div>
    <div :class="$style.tableStyle1">
      <div :class="$style.button1">
        <div :class="$style.primary">Sign up with email</div>
      </div>
    </div>
    <div :class="$style.authInner">
      <div :class="$style.frameParent">
        <div :class="$style.rectangleWrapper">
          <div :class="$style.frameChild" />
        </div>
        <div :class="$style.orContinueWith">or continue with</div>
        <div :class="$style.rectangleContainer">
          <div :class="$style.frameItem" />
        </div>
      </div>
    </div>
    <div :class="$style.tableStyle2">
      <div :class="$style.button2">
        <div :class="$style.googleWrapper">
          <img :class="$style.googleIcon" alt="" src="/google.svg" />
        </div>
        <div :class="$style.google">Google</div>
      </div>
    </div>
    <div :class="$style.byClickingContinueYouAgreWrapper">
      <div :class="$style.byClickingContinueContainer">
        <span>By clicking continue, you agree to our </span>
        <span :class="$style.termsOfService">Terms of Service</span>
        <span> and </span>
        <span :class="$style.privacyPolicy">Privacy Policy</span>
      </div>
    </div>
    <div :class="$style.navigationFooter">
      <div :class="$style.divider" />
      <div :class="$style.frameGroup">
        <div :class="$style.wingsWrapper">
          <b :class="$style.wings1">WINGS</b>
        </div>
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
    name: "Auth",
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
    width: 122px;
    position: relative;
    font-size: inherit;
    line-height: 150%;
    font-weight: 500;
    font-family: inherit;
    display: flex;
    align-items: center;
    text-shadow: 1px 0 0 #000, 0 1px 0 #000, -1px 0 0 #000, 0 -1px 0 #000;
    z-index: 1;
  }
  .symbolSwapper {
    width: 648px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-10xl) var(--padding-xl) 0px 0px;
    box-sizing: border-box;
    max-width: 100%;
    font-size: var(--font-size-13xl);
  }
  .articles {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 74px;
  }
  .tableSizeAdjuster {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-21xl) var(--padding-mid) 0px 0px;
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
  .symbolMerger {
    background-color: var(--color-rosybrown);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
  }
  .symbolMergerWrapper {
    background-color: var(--color-rosybrown);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: var(--padding-3xs);
    z-index: 1;
  }
  .pathBender {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-11xl) var(--padding-4xs) 0px 0px;
  }
  .hotels {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 62px;
  }
  .shapeColorPicker {
    width: 93px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-20xl) var(--padding-xl) 0px 0px;
    box-sizing: border-box;
  }
  .cruises {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 73px;
  }
  .tableSizeAdjuster1 {
    width: 107px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-21xl) var(--padding-xl) 0px 0px;
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
  }
  .italicController {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-10xl) 0px 0px;
    font-size: var(--small-text-size);
    color: var(--color-rosybrown);
  }
  .navigation {
    flex: 1;
    background-color: var(--color-rosybrown);
    overflow: hidden;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-8xl) var(--padding-3xs);
    box-sizing: border-box;
    gap: var(--gap-sm);
    max-width: 100%;
  }
  .linkCollection {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px var(--padding-41xl);
    box-sizing: border-box;
    max-width: 100%;
    font-size: var(--body-text-size);
  }
  .createAnAccount {
    position: relative;
    letter-spacing: -0.01em;
    line-height: 150%;
    font-weight: 600;
  }
  .logicGate {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl);
    text-align: center;
    font-size: var(--subheading-size);
  }
  .enterYourEmail {
    position: relative;
    line-height: 150%;
  }
  .inputFilter {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl) var(--padding-xl) var(--padding-2xl);
    text-align: center;
  }
  .label {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    max-width: 100%;
  }
  .field {
    width: 400px;
    border-radius: var(--br-5xs);
    background-color: var(--color-white);
    border: 1px solid var(--color-gainsboro-300);
    box-sizing: border-box;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-10xs) var(--padding-mini);
    max-width: 100%;
  }
  .tableStyle {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl) var(--padding-xs) var(--padding-2xl);
    box-sizing: border-box;
    max-width: 100%;
    font-size: var(--body-text-size);
    color: var(--color-gray);
  }
  .primary {
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .button1 {
    width: 400px;
    border-radius: var(--br-5xs);
    background-color: var(--color-black);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: var(--padding-5xs) var(--padding-xl);
    box-sizing: border-box;
    white-space: nowrap;
    max-width: 100%;
  }
  .tableStyle1 {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl) var(--padding-xl) var(--padding-2xl);
    box-sizing: border-box;
    max-width: 100%;
    color: var(--color-white);
  }
  .frameChild {
    align-self: stretch;
    height: 1px;
    position: relative;
    background-color: var(--color-gainsboro-100);
  }
  .rectangleWrapper {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-xs-5) 0px 0px;
    box-sizing: border-box;
    min-width: 84px;
  }
  .orContinueWith {
    position: relative;
    line-height: 150%;
    display: inline-block;
    min-width: 123px;
  }
  .frameItem {
    align-self: stretch;
    height: 1px;
    position: relative;
    background-color: var(--color-gainsboro-100);
  }
  .rectangleContainer {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-xs-5) 0px 0px;
    box-sizing: border-box;
    min-width: 84px;
  }
  .frameParent {
    width: 400px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    gap: var(--gap-5xs);
    max-width: 100%;
  }
  .authInner {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl) var(--padding-xl) var(--padding-2xl);
    box-sizing: border-box;
    max-width: 100%;
    text-align: center;
    color: var(--color-gray);
  }
  .googleIcon {
    width: 20px;
    height: 20px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .googleWrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-11xs) 0px 0px;
  }
  .google {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 55px;
  }
  .button2 {
    width: 400px;
    border-radius: var(--br-5xs);
    background-color: var(--color-whitesmoke);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-5xs) var(--padding-sm);
    box-sizing: border-box;
    gap: var(--gap-119xl-5);
    max-width: 100%;
  }
  .tableStyle2 {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl) var(--padding-xl) var(--padding-2xl);
    box-sizing: border-box;
    max-width: 100%;
  }
  .termsOfService {
    color: var(--color-black);
  }
  .privacyPolicy {
    color: var(--color-black);
  }
  .byClickingContinueContainer {
    width: 400px;
    position: relative;
    line-height: 150%;
    display: inline-block;
    flex-shrink: 0;
    max-width: 100%;
  }
  .byClickingContinueYouAgreWrapper {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl) var(--padding-160xl) var(--padding-2xl);
    box-sizing: border-box;
    max-width: 100%;
    text-align: center;
    color: var(--color-gray);
  }
  .divider {
    width: 1281px;
    height: 1px;
    position: relative;
    border-top: 1px solid var(--color-gainsboro-100);
    box-sizing: border-box;
    max-width: 100%;
  }
  .wings1 {
    position: relative;
    line-height: 150%;
    display: inline-block;
    min-width: 84px;
  }
  .wingsWrapper {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-xl) 0px 0px;
    box-sizing: border-box;
    min-width: 776px;
    max-width: 100%;
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
  .frameGroup {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
    max-width: 100%;
  }
  .navigationFooter {
    align-self: stretch;
    background-color: var(--color-rosybrown);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-12xs) var(--padding-smi) var(--padding-10xl)
      var(--padding-61xl);
    box-sizing: border-box;
    gap: var(--gap-31xl);
    max-width: 100%;
    font-size: var(--subheading-size);
  }
  .auth {
    width: 1480px;
    background-color: var(--color-gainsboro-400);
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: flex-start;
    padding: 0px var(--padding-12xs) 0px 0px;
    box-sizing: border-box;
    gap: var(--gap-9xs);
    max-width: 100%;
    text-align: left;
    font-size: var(--small-text-size);
    color: var(--color-black);
    font-family: var(--small-text);
  }

  @media screen and (max-width: 2025px) {
    .wings {
      font-size: var(--font-size-7xl);
      line-height: 38px;
    }

    .navigation {
      flex-wrap: wrap;
    }

    .wingsWrapper {
      min-width: 100%;
    }

    .frameGroup {
      flex-wrap: wrap;
    }

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

    .createAnAccount {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .label {
      font-size: var(--small-text-size);
      line-height: 24px;
    }

    .frameParent {
      flex-wrap: wrap;
    }

    .wings1 {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }
  }
</style>
