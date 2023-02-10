<script setup lang="ts">
import WelcomeItem from "./WelcomeItem.vue";
import DocumentationIcon from "./icons/IconDocumentation.vue";
import ToolingIcon from "./icons/IconTooling.vue";
import EcosystemIcon from "./icons/IconEcosystem.vue";
import CommunityIcon from "./icons/IconCommunity.vue";
import SupportIcon from "./icons/IconSupport.vue";
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Better than a recipe</template>

    This resource is more than a recipe. It's a toolbox + guide to help you bake a pizza at home.

    The goal is to minimize the time spent thinking about pizza, while maximizing the flavor and ingrediant quality, so you can spend more time eating pizza.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Ecosystem</template>

    It will eventually include:

    <ul>
      <li>Recommended Equipment</li>
      <li>Ingrediant List</li>
      <li>Dough Hydration Calculator</li>
      <li>Baking wizard with easy to follow steps</li>
      <li>Kitchen Timers</li>
      <li>Notifications!</li>
      <li>Personal Pizza Database to track your progress</li>
    </ul>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Tooling</template>

    Baking a pizza is easier with the right tools. We recommend checking that you have all the following tools before
    you get started:
    <form id="tools-list">
      <div>
        <input type="checkbox" name="Oven" id="oven">
        <label for="oven">Oven</label>
      </div>
      <div>
        <input type="checkbox" name="Pizza flour" id="pizza-flour">
        <label for="pizza-flour">Pizza flour</label>
      </div>
      <div>
        <input type="checkbox" name="Yeast" id="yeast">
        <label for="yeast">Yeast</label>
      </div>
      <div>
        <input type="checkbox" name="Bread Machine" id="bread-machine">
        <label for="bread-machine">Bread Machine</label>
      </div>
      <div>
        <input type="checkbox" name="Olive Oil" id="olive-oil">
        <label for="olive-oil">Olive Oil</label>
      </div>
    </form>
  </WelcomeItem>
  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Community</template>

    Got stuck? Ask your question on
    <a href="https://chat.vuejs.org" target="_blank" rel="noopener">Pizza Land</a>, our official Discord server, or
    <a href="https://stackoverflow.com/questions/tagged/vue.js" target="_blank" rel="noopener">Cooking forum reddit</a>. You
    should also subscribe to
    <a href="https://news.vuejs.org" target="_blank" rel="noopener">famous pizza chef</a>
    <!-- TODO: change links -->
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Support BakeA.Pizza</template>

    This project runs off of a passion for pizza. If you'd like to support the project, you can buy equipment off our amazon referral links, or donate money for pizza flour to your local foodbank.
  </WelcomeItem>
</template>

<style scoped>
#tools-list {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 1rem;
}
</style>