<script lang="ts">
    import { onMount } from "svelte";

    const to = "https://docs.google.com/forms/d/e/1FAIpQLSc6H3qFJwXHeGpX9P_5sGId8cpDyQCRv0IPGPbwS5m2RhOswQ/viewform?usp=sf_link";
    
    onMount(async () => {
        window.location.href = to;
    });
</script>

<svelte:head>
    <meta http-equiv="Refresh" content="0; url='{to}'" />
</svelte:head>

<a href={to}>Redirecting to {to}</a>