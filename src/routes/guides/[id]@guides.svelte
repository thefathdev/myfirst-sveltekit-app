<script context="module">
  export async function load({ fetch, params }) {
    const id = params.id;
    const res = await fetch(`https://jsonplaceholder.typicode.com/posts/${id}`);
    const data = await res.json();

    if (res.ok) {
      return {
        props: {
          guide: data,
        },
      };
    }

    return {
      status: 301,
      // error: new Error("Could not fetch the guide"),
      redirect: "/guides",
    };
  }
</script>

<script>
  export let guide;
</script>

<div class="guide">
  <h2>{guide.title}</h2>
  <p>{guide.body}</p>
</div>

<style>
  .guide {
    margin: 2em 0;
    border: 1px dotted black;
    padding-inline: 1em;
  }
</style>
