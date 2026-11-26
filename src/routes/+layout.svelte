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

    :global(h1){
        font-size: 3.6rem;
    }
    :global(h2){
        font-size: 2.4rem;
    }
    :global(h3){
        font-size: 1.2rem;
    }
    
    :global(section) {
        margin: 4rem 0rem 12rem 0rem;
    }

    :global(a) {
        color: #ffffff;
        text-decoration: none;
    }
    a:hover {
        color: #33bdeb;
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
        background-color: #56394D;
        color: #D7D7EA;
        padding: 0.8rem 1.6rem;
        border: none;
        border-radius: 0.2rem;
        cursor: pointer;
        text-align: center;
    }
    :global(.btn:hover) {
        background-color: #104239;
    }
    
    :global(.card) {
        padding: 2rem;
        background-color: #CFCFE2;
        overflow: hidden;
        max-width: 48rem;
        border-radius: 0.25rem;
        box-shadow:
            0 10px 15px -3px rgb(0 0 0 / 0.1),
            0 4px 6px -4px rgb(0 0 0 / 0.1); 
    }

    :global(.grid){
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(384px, 1fr));
        gap: 2rem;
    }
</style>
