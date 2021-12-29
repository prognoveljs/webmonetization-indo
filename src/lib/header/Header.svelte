<script lang="ts">
  import { page } from "$app/stores";
  import logo from "./svelte-logo.svg";
</script>

<header>
  <div class="corner">
    <a href="https://kit.svelte.dev">
      <img src={logo} alt="SvelteKit" />
    </a>
  </div>

  <nav>
    <a href=".">Home</a>
    <a href="apa-itu-web-monetization">Apa itu Web Monetization API?</a>
    <a href="eksplor-web-monetization">Eksplor Web Monetization API</a>
    <a href="podcast">Nonton podcast kita</a>
  </nav>
</header>

<style lang="scss">
  header {
    display: flex;
    justify-content: space-between;
  }

  .corner {
    width: 3em;
    height: 3em;
    a {
      display: flex;
      align-items: center;
      justify-content: center;
      width: 100%;
      height: 100%;
    }
    img {
      width: 2em;
      height: 2em;
      object-fit: contain;
    }
  }

  nav {
    display: flex;
    justify-content: center;
    --background: rgba(255, 255, 255, 0.7);
    margin: {
      top: 0.5em;
      right: 0.5em;
    }

    a {
      display: flex;
      height: 100%;
      align-items: center;
      padding: 0 1em;
      color: var(--heading-color);
      font-weight: 700;
      font-size: 0.8rem;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      text-decoration: none;
      transition: color 0.2s linear;
      &:hover {
        color: var(--accent-color);
      }
    }
  }
</style>
