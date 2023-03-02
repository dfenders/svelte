<script>
    import '../main.css';    

    import Header from '$lib/header.svelte';
    import Navigation from '$lib/navigation.svelte';
    import Footer from '$lib/footer.svelte';
</script>

<Header />
<Navigation />

<div class="main-content">
    <slot /> <!-- page specific content -->
</div>

<Footer />