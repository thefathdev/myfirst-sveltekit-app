<script>
  import Title from "$lib/title.svelte";
  import "../global.css";
  let title = "SvelteKit Guides";
</script>

<header>
  <Title {title} />
  <nav class="links">
    <a href="/">Home</a>
    <a href="/about">About</a>
    <a href="/guides">guides</a>
  </nav>
</header>
<main>
  <!-- page content -->
  <slot />
</main>
<footer>
  <p>&copy Copyright 2022 whatTheFath</p>
</footer>

<style>
  header,
  footer {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }

  main {
    text-align: center;
    max-width: 75ch;
    margin-inline: auto;
    margin-bottom: 2em;
  }

  .links {
    display: flex;
    gap: 1em;
  }
</style>
