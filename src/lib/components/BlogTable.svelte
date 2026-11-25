<script>
    let { articles = [] } = $props();
    function navigateToPost(slug) {
        window.location.href = `/blog/${slug}`;
    }
</script>

<section>
    <h2>Artículos recientes del Blog</h2>
    <div class="grid">
        {#each articles as post}
            <div
                class="card clickable-card"
                onclick={() => navigateToPost(post.slug)}
            >
                <h2>{post.title}</h2>
                <span>{post.category}</span>
                <p>{post.description}</p>
            </div>
        {/each}
    </div>
</section>

<style>
    .clickable-card {
        cursor: pointer;
    }
</style>
