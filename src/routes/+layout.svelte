<script>
  import "../app.css";
  import Nav from "../components/nav.svelte";
</script>

<Nav />
<slot />

<style lang="postcss">
  :global(body) {
    background-color: theme(colors.slate.800);
    min-height: 100vh;
    color: theme(colors.slate.300);
  }
</style>
