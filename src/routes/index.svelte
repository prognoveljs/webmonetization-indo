<script context="module" lang="ts">
  export const prerender = true;
</script>

<script lang="ts">
  import HomeFeatures from "$lib/home-page/HomeFeatures.svelte";
  import HomeHero from "$lib/home-page/HomeHero.svelte";
</script>

<svelte:head>
  <title>Home</title>
</svelte:head>

<HomeHero />

<HomeFeatures />
