<template>
  <div :class="$style.landingPage">
    <div :class="$style.navigation">
      <frame />
      <div :class="$style.subtree">
        <div :class="$style.branchingFactor">
          <div :class="$style.depthLevel">
            <div :class="$style.frameParent">
              <div :class="$style.articlesWrapper">
                <div :class="$style.articles">Articles</div>
              </div>
              <div :class="$style.frameWrapper">
                <div :class="$style.frameContainer">
                  <div :class="$style.connectedComponentsWrapper">
                    <div :class="$style.connectedComponents">
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
            </div>
          </div>
          <div :class="$style.button">
            <div :class="$style.signUp">Sign Up</div>
          </div>
        </div>
      </div>
    </div>
    <div :class="$style.treeDiameter">
      <div :class="$style.treeShape">
        <h1 :class="$style.goBoldly">GO BOLDLY</h1>
        <div :class="$style.loveInspiringTravel">
          Love inspiring travel stories ? Get the latest news delivered to your
          inbox.
        </div>
      </div>
    </div>
    <div :class="$style.binarySearchTree">
      <div :class="$style.aVLTree">
        <RedBlackTree
          wakatobi="Wakatobi"
          sandAndSerenityAtWakatobi="Sand and Serenity At Wakatobi’s Turtle Beach"
        />
        <img
          :class="$style.images1Icon"
          loading="lazy"
          alt=""
          src="/images-1@2x.png"
        />
      </div>
    </div>
    <div :class="$style.forestSegmentation">
      <div :class="$style.connectedComponentsLabeling">
        <img
          :class="$style.marqueeTravelParis800x4501Icon"
          loading="lazy"
          alt=""
          src="/marqueetravelparis800x450-1@2x.png"
        /><RedBlackTree
          wakatobi="Paris"
          sandAndSerenityAtWakatobi="31 things to do in Paris during the 2024 Olympics"
          propPadding="var(--padding-76xl) 0px 0px"
          propAlignSelf="unset"
        />
      </div>
    </div>
    <div :class="$style.graphTraversal">
      <div :class="$style.graphColoring">
        <div :class="$style.biconnectedComponents">
          <h1 :class="$style.articles1">Articles</h1>
        </div>
        <div :class="$style.cutVertices">
          <div :class="$style.connectivity">
            <div :class="$style.graphRepresentation">
              <div :class="$style.dataAggregatorParent">
                <div :class="$style.dataAggregator">
                  <div :class="$style.conditionBranch">
                    <h1 :class="$style.inputContainer">+</h1>
                    <div :class="$style.outputCollector">
                      <div :class="$style.palau">Palau</div>
                    </div>
                  </div>
                  <div :class="$style.valueComparator">
                    <a
                      :class="$style.terrificReasonsTo"
                      href="https://www.vacationstravel.com/palau/"
                      target="_blank"
                      >14 terrific reasons to visit Palau now</a
                    >
                  </div>
                </div>
                <div :class="$style.functionCallTree">
                  <h1 :class="$style.h1">+</h1>
                  <div :class="$style.dataProcessor">
                    <div :class="$style.patagonia">Patagonia</div>
                  </div>
                </div>
              </div>
            </div>
            <div :class="$style.frameGroup">
              <div :class="$style.frameDiv">
                <div :class="$style.parent">
                  <h1 :class="$style.h11">+</h1>
                  <div :class="$style.sydneyWrapper">
                    <div :class="$style.sydney">Sydney</div>
                  </div>
                </div>
                <div :class="$style.jonahsRestaurantBoutiqueWrapper">
                  <div :class="$style.jonahsRestaurant">
                    Jonah’s Restaurant & Boutique Hotel is ripe for romance
                  </div>
                </div>
              </div>
              <div :class="$style.group">
                <h1 :class="$style.h12">+</h1>
                <div :class="$style.indiaWrapper">
                  <div :class="$style.india">India</div>
                </div>
              </div>
            </div>
          </div>
          <div :class="$style.discoverPatagoniaWithAbercrParent">
            <div :class="$style.discoverPatagoniaWith">
              Discover Patagonia with Abercrombie & Kent
            </div>
            <div :class="$style.theVtGuideToNorthernIndiWrapper">
              <div :class="$style.theVtGuide">
                The V&T guide to Northern India
              </div>
            </div>
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
  import RedBlackTree from "./RedBlackTree.vue";
  import NavigationFooter from "./NavigationFooter.vue";

  export default defineComponent({
    name: "LandingPage",
    components: { Frame, RedBlackTree, NavigationFooter },
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
    padding: var(--padding-3xs) 0px 0px;
  }
  .destinations {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 120px;
  }
  .connectedComponents {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
  }
  .connectedComponentsWrapper {
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
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-3xs) 0px 0px;
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
    padding: var(--padding-3xs) var(--padding-lg) 0px 0px;
  }
  .cruises {
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    min-width: 73px;
  }
  .cruisesWrapper {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-3xs) 0px 0px;
  }
  .frameParent {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-mid);
  }
  .depthLevel {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-12xs) 0px 0px;
    box-sizing: border-box;
    max-width: 100%;
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
  .branchingFactor {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-29xl);
    max-width: 100%;
  }
  .subtree {
    width: 584px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-10xl) 0px 0px;
    box-sizing: border-box;
    max-width: 100%;
    font-size: var(--body-text-size);
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
    font-size: var(--font-size-13xl);
  }
  .goBoldly {
    margin: 0;
    align-self: stretch;
    position: relative;
    font-size: inherit;
    letter-spacing: -0.02em;
    font-weight: 700;
    font-family: inherit;
  }
  .loveInspiringTravel {
    align-self: stretch;
    position: relative;
    font-size: var(--subheading-size);
    line-height: 150%;
    color: var(--color-gray);
  }
  .treeShape {
    width: 912.2px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xl);
    max-width: 100%;
  }
  .treeDiameter {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl) var(--padding-43xl);
    box-sizing: border-box;
    max-width: 100%;
    text-align: center;
    font-size: var(--title-size);
  }
  .images1Icon {
    height: 401px;
    flex: 1;
    position: relative;
    max-width: 100%;
    overflow: hidden;
    object-fit: cover;
    min-width: 448px;
  }
  .aVLTree {
    width: 1377.3px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    gap: var(--gap-109xl-3);
    max-width: 100%;
  }
  .binarySearchTree {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-10xl) var(--padding-xs) var(--padding-xl);
    box-sizing: border-box;
    max-width: 100%;
  }
  .marqueeTravelParis800x4501Icon {
    width: 689px;
    position: relative;
    max-height: 100%;
    object-fit: cover;
    max-width: 100%;
  }
  .connectedComponentsLabeling {
    width: 1384.3px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    max-width: 100%;
    gap: var(--gap-xl);
  }
  .forestSegmentation {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    padding: 0px var(--padding-xl) var(--padding-6xs) var(--padding-3xl);
    box-sizing: border-box;
    max-width: 100%;
  }
  .articles1 {
    margin: 0;
    flex: 1;
    position: relative;
    font-size: inherit;
    line-height: 110%;
    font-weight: 600;
    font-family: inherit;
    display: inline-block;
    max-width: 100%;
  }
  .biconnectedComponents {
    width: 635px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-8xs);
    box-sizing: border-box;
    max-width: 100%;
  }
  .inputContainer {
    margin: 0;
    width: 27px;
    position: relative;
    font-size: inherit;
    line-height: 110%;
    font-weight: 600;
    font-family: inherit;
    display: inline-block;
  }
  .palau {
    align-self: stretch;
    position: relative;
    line-height: 150%;
  }
  .outputCollector {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-6xs) 0px 0px;
    box-sizing: border-box;
    min-width: 335px;
    max-width: 100%;
    font-size: var(--subheading-size);
    color: var(--color-black);
  }
  .conditionBranch {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-8xs-3);
    max-width: 100%;
  }
  .terrificReasonsTo {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 500;
    color: inherit;
    display: inline-block;
    text-decoration: none;
    max-width: 100%;
  }
  .valueComparator {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px 0px var(--padding-12xl-3);
    box-sizing: border-box;
    max-width: 100%;
    font-size: var(--body-text-size);
  }
  .dataAggregator {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-6xs);
    max-width: 100%;
  }
  .h1 {
    margin: 0;
    width: 27px;
    position: relative;
    font-size: inherit;
    line-height: 110%;
    font-weight: 600;
    font-family: inherit;
    display: inline-block;
  }
  .patagonia {
    align-self: stretch;
    position: relative;
    line-height: 150%;
  }
  .dataProcessor {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-5xs) 0px 0px;
    box-sizing: border-box;
    min-width: 335px;
    max-width: 100%;
    font-size: var(--subheading-size);
    color: var(--color-black);
  }
  .functionCallTree {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-8xs-3);
    max-width: 100%;
  }
  .dataAggregatorParent {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-21xl);
    max-width: 100%;
  }
  .graphRepresentation {
    width: 546.3px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-base) 0px 0px;
    box-sizing: border-box;
    min-width: 546.3000000000002px;
    max-width: 100%;
  }
  .h11 {
    margin: 0;
    width: 27px;
    position: relative;
    font-size: inherit;
    line-height: 110%;
    font-weight: 600;
    font-family: inherit;
    display: inline-block;
  }
  .sydney {
    align-self: stretch;
    position: relative;
    line-height: 150%;
  }
  .sydneyWrapper {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-5xs) 0px 0px;
    box-sizing: border-box;
    min-width: 333px;
    max-width: 100%;
    font-size: var(--subheading-size);
    color: var(--color-black);
  }
  .parent {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-4xs-6);
    max-width: 100%;
  }
  .jonahsRestaurant {
    flex: 1;
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: inline-block;
    max-width: 100%;
  }
  .jonahsRestaurantBoutiqueWrapper {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px 0px var(--padding-16xl-6);
    box-sizing: border-box;
    max-width: 100%;
    font-size: var(--body-text-size);
  }
  .frameDiv {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-5xs);
    max-width: 100%;
  }
  .h12 {
    margin: 0;
    width: 27px;
    position: relative;
    font-size: inherit;
    line-height: 110%;
    font-weight: 600;
    font-family: inherit;
    display: inline-block;
  }
  .india {
    align-self: stretch;
    position: relative;
    line-height: 150%;
  }
  .indiaWrapper {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-6xs) 0px 0px;
    box-sizing: border-box;
    min-width: 333px;
    max-width: 100%;
    font-size: var(--subheading-size);
    color: var(--color-black);
  }
  .group {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-4xs-6);
    max-width: 100%;
  }
  .frameGroup {
    width: 548.6px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-22xl);
    min-width: 548.6000000000004px;
    max-width: 100%;
  }
  .connectivity {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    max-width: 100%;
    gap: var(--gap-xl);
  }
  .discoverPatagoniaWith {
    width: 515px;
    position: relative;
    line-height: 150%;
    font-weight: 500;
    display: flex;
    align-items: center;
    flex-shrink: 0;
    max-width: 100%;
  }
  .theVtGuide {
    align-self: stretch;
    position: relative;
    line-height: 150%;
    font-weight: 500;
  }
  .theVtGuideToNorthernIndiWrapper {
    width: 513px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: var(--padding-mini) 0px 0px;
    box-sizing: border-box;
    max-width: 100%;
  }
  .discoverPatagoniaWithAbercrParent {
    width: 1318.3px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    max-width: 100%;
    gap: var(--gap-xl);
    margin-top: -8px;
    font-size: var(--body-text-size);
  }
  .cutVertices {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: flex-start;
    max-width: 100%;
    color: var(--color-gray);
  }
  .graphColoring {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-4xs);
    max-width: 100%;
  }
  .graphTraversal {
    width: 1499.6px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-56xl) var(--padding-41xl);
    box-sizing: border-box;
    max-width: 100%;
  }
  .landingPage {
    align-self: stretch;
    background-color: var(--color-gainsboro-400);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    gap: var(--gap-101xl);
    max-width: 100%;
    text-align: left;
    font-size: var(--heading-size);
    color: var(--color-black);
    font-family: var(--small-text);
  }

  @media screen and (max-width: 2025px) {
    .frameParent {
      display: none;
    }

    .branchingFactor {
      gap: var(--gap-5xl);
    }

    .navigation {
      flex-wrap: wrap;
      padding-right: var(--padding-21xl);
      box-sizing: border-box;
    }

    .goBoldly {
      font-size: var(--font-size-32xl);
    }

    .images1Icon {
      min-width: 100%;
    }

    .aVLTree {
      flex-wrap: wrap;
      gap: var(--gap-13xl);
    }

    .marqueeTravelParis800x4501Icon {
      flex: 1;
    }

    .connectedComponentsLabeling {
      flex-wrap: wrap;
      justify-content: center;
    }

    .articles1 {
      font-size: var(--font-size-13xl);
      line-height: 35px;
    }

    .inputContainer {
      font-size: var(--font-size-13xl);
      line-height: 35px;
    }

    .conditionBranch {
      flex-wrap: wrap;
    }

    .h1 {
      font-size: var(--font-size-13xl);
      line-height: 35px;
    }

    .functionCallTree {
      flex-wrap: wrap;
    }

    .dataAggregatorParent {
      gap: var(--gap-xl);
    }

    .graphRepresentation {
      flex: 1;
      min-width: 100%;
    }

    .h11 {
      font-size: var(--font-size-13xl);
      line-height: 35px;
    }

    .parent {
      flex-wrap: wrap;
    }

    .h12 {
      font-size: var(--font-size-13xl);
      line-height: 35px;
    }

    .group {
      flex-wrap: wrap;
    }

    .frameGroup {
      flex: 1;
      gap: var(--gap-xl);
      min-width: 100%;
    }

    .connectivity {
      flex-wrap: wrap;
    }

    .discoverPatagoniaWithAbercrParent {
      flex-wrap: wrap;
    }

    .graphTraversal {
      padding-left: var(--padding-18xl);
      padding-right: var(--padding-18xl);
      box-sizing: border-box;
    }

    .landingPage {
      gap: var(--gap-41xl);
    }
  }
  @media screen and (max-width: 450px) {
    .goBoldly {
      font-size: var(--font-size-19xl);
    }

    .loveInspiringTravel {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .aVLTree {
      gap: var(--gap-base);
    }

    .articles1 {
      font-size: var(--subheading-size);
      line-height: 26px;
    }

    .inputContainer {
      font-size: var(--subheading-size);
      line-height: 26px;
    }

    .palau {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .terrificReasonsTo {
      font-size: var(--small-text-size);
      line-height: 24px;
    }

    .h1 {
      font-size: var(--subheading-size);
      line-height: 26px;
    }

    .patagonia {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .h11 {
      font-size: var(--subheading-size);
      line-height: 26px;
    }

    .sydney {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .jonahsRestaurant {
      font-size: var(--small-text-size);
      line-height: 24px;
    }

    .h12 {
      font-size: var(--subheading-size);
      line-height: 26px;
    }

    .india {
      font-size: var(--font-size-lgi);
      line-height: 29px;
    }

    .discoverPatagoniaWith {
      font-size: var(--small-text-size);
      line-height: 24px;
    }

    .theVtGuide {
      font-size: var(--small-text-size);
      line-height: 24px;
    }

    .landingPage {
      gap: var(--gap-11xl);
    }
  }
</style>
