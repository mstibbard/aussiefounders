<script lang="ts">
  import '../app.css';
  import { dev } from '$app/env';
</script>

<svelte:head>
  {#if !dev}
    <script
      defer
      data-domain="aussiefounders.com.au"
      src="https://plausible.io/js/plausible.js"></script>
  {/if}
</svelte:head>

<div class="max-w-3xl md:max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 lg:py-16">
  <slot />
</div>
