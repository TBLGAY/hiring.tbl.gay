<script lang="ts">
    import { onMount } from "svelte";

    const to = "https://docs.google.com/forms/d/e/1FAIpQLSfNGrTDUheW_pYbG79wqXHv6vLTkBCOKsv6X4Sk5i742rgqDg/viewform?usp=sf_link";
    
    onMount(async () => {
        window.location.href = to;
    });
</script>

<svelte:head>
    <meta http-equiv="Refresh" content="0; url='{to}'" />
</svelte:head>

<a href={to}>Redirecting to {to}</a>