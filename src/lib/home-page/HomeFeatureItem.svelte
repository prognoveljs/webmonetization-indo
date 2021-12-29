<script lang="ts">
  export let title: string;
</script>

<section>
  <strong>{title}</strong>
  <slot />
</section>

<style lang="scss">
  section {
    padding: 2em 1.25em;
    border-radius: 8px;
    background-color: #fff;
    box-shadow: 1.3px 2.6px 3.6px rgba(0, 0, 0, 0.014),
      3.6px 7.1px 10px rgba(0, 0, 0, 0.02),
      8.7px 17.2px 24.1px rgba(0, 0, 0, 0.026),
      29px 57px 80px rgba(0, 0, 0, 0.04);

    strong {
      font-size: 1.3em;
      display: block;
      line-height: 1;
      margin-bottom: 0.7em;
    }
  }
</style>
