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

    This resource is more than a recipe. It's a toolbox + guide to help you bake a pizza.
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
        <label for="pizza-flour">Pizza</label>
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
      <EcosystemIcon />
    </template>
    <template #heading>Ecosystem</template>

    Get official tools and libraries for your project:
    <a href="https://pinia.vuejs.org/" target="_blank" rel="noopener">Pinia</a>,
    <a href="https://router.vuejs.org/" target="_blank" rel="noopener">Vue Router</a>,
    <a href="https://test-utils.vuejs.org/" target="_blank" rel="noopener">Vue Test Utils</a>, and
    <a href="https://github.com/vuejs/devtools" target="_blank" rel="noopener">Vue Dev Tools</a>. If you need more
    resources, we suggest paying
    <a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">Awesome Vue</a>
    a visit.
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

    As an independent project, Vue relies on community backing for its
    sustainability. You can help us by
    <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">becoming a sponsor</a>.
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