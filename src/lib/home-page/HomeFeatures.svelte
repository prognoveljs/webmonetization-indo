<script lang="ts">
  import HomeFeatureItem from "./HomeFeatureItem.svelte";
</script>

<h2>Apa itu Web Monetization API?</h2>
<article>
  <HomeFeatureItem title="💸 Dapat uang secara real-time">
    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aperiam modi
    distinctio deserunt reprehenderit quos quae et fuga incidunt in eligendi.
    Iusto suscipit, sequi sit magni voluptates possimus. Quae, similique illum.
  </HomeFeatureItem>
  <HomeFeatureItem title="💱 Agnostic mata uang">
    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aperiam modi
    distinctio deserunt reprehenderit quos quae et fuga incidunt in eligendi.
    Iusto suscipit, sequi sit magni voluptates possimus. Quae, similique illum.
  </HomeFeatureItem>
  <HomeFeatureItem title="🏆 Potensi juara">
    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aperiam modi
    distinctio deserunt reprehenderit quos quae et fuga incidunt in eligendi.
    Iusto suscipit, sequi sit magni voluptates possimus. Quae, similique illum.
  </HomeFeatureItem>
  <HomeFeatureItem title="👩‍🎨 Kreator dan komunitas nomor satu">
    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Aperiam modi
    distinctio deserunt reprehenderit quos quae et fuga incidunt in eligendi.
    Iusto suscipit, sequi sit magni voluptates possimus. Quae, similique illum.
  </HomeFeatureItem>
</article>

<style lang="scss">
  h2 {
    text-align: center;
    font-size: 2em;
    font-weight: 700;
    margin-top: 3em;
  }
  article {
    $gap: 2em;
    display: flex;
    justify-content: space-between;
    gap: $gap;

    @supports not (gap: 1em) {
      :global(section:not(:last-child)) {
        margin-right: $gap;
      }
    }
  }
</style>
