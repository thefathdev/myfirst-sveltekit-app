<script>
  export let title = "title";
</script>

<div class="title">
  <img src="/cling.svg" alt="Site logos" />
  <h1>{title}</h1>
</div>

<style>
  .title {
    display: flex;
    justify-content: center;
    align-items: center;
    border: 4px solid black;
    padding: 1em 4em;
    border-radius: 1rem;
    box-shadow: 8px 8px 0 0 black;
    margin-bottom: 2em;
    margin-top: 0.5em;
  }

  .title img {
    display: inline-block;
    aspect-ratio: 1;
    width: 4em;
    height: auto;
  }

  .title h1 {
    margin-left: 0.5em;
  }
</style>
