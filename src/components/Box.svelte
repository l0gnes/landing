<script lang="ts">
    let { children } = $props();
</script>

<div class="p-2 border border-neutral-600 border-l-neutral-500 border-t-neutral-500 bg-neutral-900 drop-shadow-md drop-shadow-black">
    {@render children()}
</div>