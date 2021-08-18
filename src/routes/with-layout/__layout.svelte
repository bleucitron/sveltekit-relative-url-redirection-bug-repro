<script context="module">
  export function load({ page }) {
    if (page.path === '/with-layout') {
      return {
        status: 301,
        // This should redirect to /with-layout/target but redirects to /target => BUG
        redirect: './target',
      };
    }
    return {};
  }
</script>

<slot />
