<script>
  import Title from "$lib/title.svelte";
  import "../global.css";
  let title = "Intro to SvelteKit";
</script>

<header>
  <Title {title} />
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
  }

  main {
    text-align: center;
    max-width: 75ch;
    margin-inline: auto;
    margin-bottom: 2em;
  }
</style>
