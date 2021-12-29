<script lang="ts">
  import Header from "$lib/header/Header.svelte";
  import "../app.css";
</script>

<svelte:head>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Dosis:wght@300;400;700&display=swap"
    rel="stylesheet"
  />
</svelte:head>

<Header />

<main>
  <slot />
</main>

<footer>...</footer>

<style lang="scss">
  body::before {
    content: "";
    width: 80vw;
    height: 100vh;
    position: absolute;
    top: 0;
    left: 10vw;
    z-index: -1;
    background: radial-gradient(
      50% 50% at 50% 50%,
      var(--pure-white) 0%,
      rgba(255, 255, 255, 0) 100%
    );
    opacity: 0.05;
  }
  main {
    flex: 1;
    display: flex;
    flex-direction: column;
    padding: 1rem;
    width: 100%;
    max-width: 1024px;
    margin: 0 auto;
    box-sizing: border-box;
  }

  footer {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 40px;
  }

  footer a {
    font-weight: bold;
  }

  @media (min-width: 480px) {
    footer {
      padding: 40px 0;
    }
  }
</style>
