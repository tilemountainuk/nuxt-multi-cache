<template>
  <div class="main-layout">
    <header>
<!--      <RenderCacheable cache-key="navbar" :async-data-keys="['navbar']">-->
        <Navbar />
<!--      </RenderCacheable>-->
    </header>
    <main>
      <slot />
      <api-playground />
    </main>
  </div>
</template>

<style>
.main-layout {
  display: grid;
  grid-template-columns: 20rem 1fr;
  grid-gap: 2rem;
  padding: 2rem;
}
</style>
<script setup lang="ts">
import ApiPlayground from "../components/apiPlayground.vue";
</script>
