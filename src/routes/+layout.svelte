<script>
    import Navigation from '$lib/navigation.svelte';
    import Footer from '$lib/footer.svelte';
</script>

<Navigation />

<slot /> <!-- page specific content -->

<Footer />