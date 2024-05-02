<template>
  <div :class="$style.contactUs">
    <div :class="$style.navigation">
      <frame propWidth="245px" propGap="14px" />
      <div :class="$style.dataValidator">
        <nav :class="$style.dataTransformers">
          <div :class="$style.dataControllers">
            <div :class="$style.articles">Articles</div>
          </div>
          <div :class="$style.dataAggregator">
            <div :class="$style.logicGate">
              <div :class="$style.inputConnectorWrapper">
                <div :class="$style.inputConnector">
                  <div :class="$style.destinations">Destinations</div>
                </div>
              </div>
            </div>
          </div>
          <div :class="$style.dataControllers1">
            <div :class="$style.hotels">Hotels</div>
          </div>
          <div :class="$style.dataControllers2">
            <div :class="$style.cruises">Cruises</div>
          </div>
          <div :class="$style.button">
            <div :class="$style.signUp">Sign Up</div>
          </div>
        </nav>
      </div>
    </div>
    <div :class="$style.valueProcessor">
      <div :class="$style.iconLibraryParent">
        <div :class="$style.iconLibrary">
          <div :class="$style.tableStructure">
            <h1 :class="$style.contactUs1">Contact us</h1>
            <div :class="$style.colorPalette">
              <div :class="$style.doHaveAny">
                Do have any questions ? Get in touch with our team.
              </div>
            </div>
            <div :class="$style.formWrapper">
              <div :class="$style.form">
                <div :class="$style.input">
                  <div :class="$style.firstName">First name</div>
                  <div :class="$style.field">
                    <div :class="$style.label">Jane</div>
                  </div>
                </div>
                <div :class="$style.input1">
                  <div :class="$style.lastName">Last name</div>
                  <div :class="$style.field1">
                    <div :class="$style.label1">Smitherton</div>
                  </div>
                </div>
                <div :class="$style.input2">
                  <div :class="$style.emailAddress">Email address</div>
                  <div :class="$style.field2">
                    <div :class="$style.label2">email@janesfakedomain.net</div>
                  </div>
                </div>
                <div :class="$style.input3">
                  <div :class="$style.yourMessage">Your message</div>
                  <div :class="$style.field3">
                    <div :class="$style.label3">
                      Enter your question or message
                    </div>
                  </div>
                </div>
                <div :class="$style.button1">
                  <div :class="$style.submit">Submit</div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <img
          :class="$style.roadtrip15835263131Icon"
          loading="lazy"
          alt=""
          src="/roadtrip1583526313-1@2x.png"
        />
      </div>
    </div>
    <NavigationFooter />
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";
  import Frame from "./Frame.vue";
  import NavigationFooter from "./NavigationFooter.vue";

  export default defineComponent({
    name: "ContactUs",
    components: { Frame, NavigationFooter },
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
  .dataControllers {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-2xs) var(--padding-10xs) 0px 0px;
  }
  .destinations {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 120px;
  }
  .inputConnector {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
  }
  .inputConnectorWrapper {
    background-color: var(--color-rosybrown);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
  }
  .logicGate {
    background-color: var(--color-rosybrown);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: var(--padding-3xs);
    z-index: 1;
  }
  .dataAggregator {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-12xs) var(--padding-15xl) 0px 0px;
  }
  .hotels {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 62px;
  }
  .dataControllers1 {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-2xs) 0px 0px;
  }
  .cruises {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 73px;
  }
  .dataControllers2 {
    width: 107px;
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
  .dataTransformers {
    margin: 0;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-sm);
    white-space: nowrap;
    text-align: left;
    font-size: var(--body-text-size);
    color: var(--color-black);
    font-family: var(--small-text);
  }
  .dataValidator {
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
  .contactUs1 {
    margin: 0;
    width: 624px;
    position: relative;
    font-size: inherit;
    letter-spacing: -0.02em;
    font-weight: 700;
    font-family: inherit;
    display: inline-block;
    max-width: 100%;
  }
  .doHaveAny {
    flex: 1;
    position: relative;
    line-height: 150%;
    display: inline-block;
    max-width: 100%;
  }
  .colorPalette {
    width: 624px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px var(--padding-5xs);
    box-sizing: border-box;
    max-width: 100%;
    font-size: var(--subheading-size);
    color: var(--color-gray);
  }
  .firstName {
    align-self: stretch;
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .label {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .field {
    align-self: stretch;
    box-shadow: var(--button-shadow);
    border-radius: var(--br-5xs);
    background-color: var(--color-white);
    border: 1px solid var(--color-gainsboro-300);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-3xs) var(--padding-mini);
    color: var(--color-gray);
  }
  .input {
    width: 295px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .lastName {
    align-self: stretch;
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .label1 {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .field1 {
    align-self: stretch;
    box-shadow: var(--button-shadow);
    border-radius: var(--br-5xs);
    background-color: var(--color-white);
    border: 1px solid var(--color-gainsboro-300);
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-3xs) var(--padding-mini);
    color: var(--color-gray);
  }
  .input1 {
    width: 297px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
  }
  .emailAddress {
    align-self: stretch;
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .label2 {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    white-space: nowrap;
    max-width: 100%;
  }
  .field2 {
    align-self: stretch;
    box-shadow: var(--button-shadow);
    border-radius: var(--br-5xs);
    background-color: var(--color-white);
    border: 1px solid var(--color-gainsboro-300);
    box-sizing: border-box;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-3xs) var(--padding-mini);
    max-width: 100%;
    color: var(--color-gray);
  }
  .input2 {
    width: 626px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
    max-width: 100%;
  }
  .yourMessage {
    align-self: stretch;
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .label3 {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    max-width: 100%;
  }
  .field3 {
    align-self: stretch;
    box-shadow: var(--button-shadow);
    border-radius: var(--br-5xs);
    background-color: var(--color-white);
    border: 1px solid var(--color-gainsboro-300);
    box-sizing: border-box;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-3xs) var(--padding-mini) var(--padding-105xl);
    max-width: 100%;
    color: var(--color-gray);
  }
  .input3 {
    width: 626px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
    max-width: 100%;
  }
  .submit {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 68px;
  }
  .button1 {
    box-shadow: var(--button-shadow);
    border-radius: var(--br-5xs);
    background-color: var(--color-black);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: var(--padding-base) var(--padding-xl);
    font-size: var(--body-text-size);
    color: var(--color-white);
  }
  .form {
    width: 678.2px;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-33xl-2) 0px 0px;
    box-sizing: border-box;
    gap: 24px 32px;
    min-height: 488px;
    max-width: 100%;
  }
  .formWrapper {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px 0px var(--padding-6xs-7);
    box-sizing: border-box;
    max-width: 100%;
    font-size: var(--small-text-size);
  }
  .tableStructure {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xl);
    max-width: 100%;
  }
  .iconLibrary {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-9xs) 0px 0px;
    box-sizing: border-box;
    min-width: 445px;
    max-width: 100%;
  }
  .roadtrip15835263131Icon {
    width: 554px;
    position: relative;
    max-height: 100%;
    object-fit: cover;
    max-width: 100%;
  }
  .iconLibraryParent {
    flex: 1;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-155xl-1);
    max-width: 100%;
  }
  .valueProcessor {
    width: 1547px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-end;
    padding: 0px var(--padding-48xl) var(--padding-5xl);
    box-sizing: border-box;
    max-width: 100%;
    flex-shrink: 0;
  }
  .contactUs {
    align-self: stretch;
    height: 1262px;
    background-color: var(--color-gainsboro-400);
    overflow: hidden;
    flex-shrink: 0;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: flex-start;
    padding: 0px 0px var(--padding-193xl);
    box-sizing: border-box;
    gap: var(--gap-57xl);
    max-width: 100%;
    text-align: left;
    font-size: var(--title-size);
    color: var(--color-black);
    font-family: var(--small-text);
  }

  @media screen and (max-width: 2025px) {
    .dataTransformers {
      flex-wrap: wrap;
    }

    .navigation {
      flex-wrap: wrap;
      padding-right: var(--padding-21xl);
      box-sizing: border-box;
    }

    .contactUs1 {
      font-size: var(--font-size-32xl);
    }

    .form {
      gap: var(--spacing-sm);
      padding-right: var(--padding-7xl);
      box-sizing: border-box;
    }

    .iconLibrary {
      min-width: 100%;
    }

    .roadtrip15835263131Icon {
      flex: 1;
    }

    .iconLibraryParent {
      flex-wrap: wrap;
      gap: var(--gap-25xl);
    }

    .valueProcessor {
      padding-left: var(--padding-14xl);
      padding-right: var(--padding-14xl);
      box-sizing: border-box;
    }

    .contactUs {
      height: auto;
      gap: var(--gap-19xl);
      padding-bottom: var(--padding-71xl);
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

    .contactUs1 {
      font-size: var(--font-size-19xl);
    }

    .doHaveAny {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .submit {
      font-size: var(--small-text-size);
      line-height: 24px;
    }

    .iconLibraryParent {
      gap: var(--gap-3xl);
    }

    .contactUs {
      gap: var(--gap-lgi);
    }
  }
</style>
