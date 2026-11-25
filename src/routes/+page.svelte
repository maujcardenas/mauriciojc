<script>
    import HeroSection from "$lib/components/HeroSection.svelte";
    import BlogTable from "$lib/components/BlogTable.svelte";
    import Contact from "$lib/components/Contact.svelte";

    let { data } = $props();
    let articles = $derived(data.recentPosts);
</script>

<div class="layout-container">
    <HeroSection />
    <BlogTable {articles} />
    <Contact />
</div>

<style>
</style>
