<!--
Redirection from __error not working for now

See https://github.com/sveltejs/kit/pull/2127#discussion_r688317905 for actual reproduction
-->
<script context="module">
  export function load() {
    return {
      status: 301,
      // This should redirect to /with-error/target but redirects to /target => BUG
      redirect: './target',
    };
  }
</script>

<h1>Error</h1>
