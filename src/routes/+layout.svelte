<script>
    import Header from "$lib/components/Header.svelte";
    import Footer from "$lib/components/Footer.svelte";

    let { children } = $props();
</script>

<Header />
<main>
    {@render children()}
</main>
<Footer />

<style>
    :global(main) {
        padding-top: 120px; /*por el header fijo */
        min-height: calc(100vh - 200px);
    }
    :global(body) {
        margin: 0;
        padding: 0;
        font-family: "DM Sans", sans-serif;
        background-color: #D7D7EA;
        color: #080708;
    }
    :global(section) {
        margin: 4rem 0;
    }
    :global(h1, h2, h3, h4) {
        color: #080708;
        margin-bottom: 0.5rem;
    }
    :global(p, span, li) {
        color: #080708;
    }
    :global(a) {
        color: #0c325a;
        text-decoration: none;
    }
    :global(img) {
        max-width: 100%;
        height: auto;
        border-radius: 12px;
    }
    :global(.layout-container){
        max-width: 1200px;
        margin: 0 auto;
        padding: 0 2rem;
    }
    :global(.text-accent) {
        font-weight: bold;
        color: #ff7a00; /* Replace with your preferred orange shade */
        flex: 0 0 100%; /* Forces it to take up the full width (new row) on mobile */
    }
    :global(.btn) {
        display: inline-block;
        background-color: #0c325a;
        color: #ffffff;
        padding: 0.75rem 1.5rem;
        border: none;
        border-radius: 8px;
        cursor: pointer;
        text-align: center;
    }
    :global(.btn:hover) {
        /* opacity: 0.8; */
        background-color: #000000;
        /* color: #E0F2FE; */
    }
    :global(.section-title){
        margin-bottom: 2.5rem;
        font-size: 2rem;
        color: #000000;
    }
    
    :global(.card) {
        padding: 3rem;
        background-color: #080708;
        color: #080708;
        border-radius: 12px;
        overflow: hidden;
        display: flex;
        flex-direction: column;
        max-width: 760px;
    }

    :global(.grid-2){
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 2rem;
    }

</style>
