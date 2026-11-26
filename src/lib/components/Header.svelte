<script>
    import LinkedInLogo from "$lib/components/social-media/LinkedInLogo.svelte";
    import YouTubeLogo from "$lib/components/social-media/YouTubeLogo.svelte";
    import WhatsAppLogo from "$lib/components/social-media/WhatsAppLogo.svelte";
</script>

<header>
    <div class="header-container">
        <div class="logo-section">
            <a href="/" class="brand-link">mauriciojc.com </a>
        </div>

        <nav class="nav-menu">
            <a href="/">Inicio</a>
            <a href="/blog">Blog</a>
            <a href="/blog/meditacion">Meditación</a>
            <a href="/blog/recomendaciones">Recomendaciones</a>
            <a href="/blog/foto">Fotografía</a>
            <a href="/#contacto">Contacto</a>
        </nav>

        <div class="social-icons">
            <a
                href="https://www.linkedin.com/in/mauriciojc/"
                aria-label="LinkedIn"
                target="_blank"
                rel="noopener noreferrer"
            >
                <LinkedInLogo />
            </a>
            <a
                href="https://www.youtube.com/@mautematicas"
                aria-label="YouTube"
                target="_blank"
                rel="noopener noreferrer"
            >
                <YouTubeLogo />
            </a>
            <a
                href="https://wa.me/593984029541"
                aria-label="WhatsApp"
                target="_blank"
                rel="noopener noreferrer"
            >
                <WhatsAppLogo />
            </a>
        </div>
    </div>
</header>

<style>
    header {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        background-color: #104239;
        /* border-bottom: 1px solid #2a2829; */
        z-index: 1000;
        color: #d7d7ea;
    }

    .header-container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0.8rem 1.6rem;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
        gap: 2rem;
    }

    .brand-link {
        display: inline-block;
        line-height: 0;
    }

    .nav-menu {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: flex-start;
        align-items: center;
        gap: 1rem;
    }

    .social-icons {
        display: flex;
        align-items: center;
        gap: 1rem;
    }
</style>
