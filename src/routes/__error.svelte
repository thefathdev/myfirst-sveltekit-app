<script context="module">
  export function load({ error }) {
    return {
      props: { message: error.message },
    };
  }
</script>

<script>
  export let message;
</script>

<div class="error">
  <h2>Ooops!</h2>
  <p>{message}</p>
  <nav>
    <a href="/">Home</a>
    <a href="/guides">View all guides...</a>
  </nav>
</div>

<style>
  h2 {
    font-size: 3em;
    color: red;
  }

  nav {
    display: flex;
    gap: 1em;
  }

  .error {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
</style>
