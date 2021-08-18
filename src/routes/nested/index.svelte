<script context="module">
  export function load() {
    return {
      status: 301,
      // This should redirect to /nested/target but redirects to /target => BUG
      redirect: './target',
    };
  }
</script>

<h1>Nested index</h1>
