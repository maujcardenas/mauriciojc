<script>
    import LinkedInLogo from "$lib/components/social-media/LinkedInLogo.svelte";
    import YouTubeLogo from "$lib/components/social-media/YouTubeLogo.svelte";
    import WhatsAppLogo from "$lib/components/social-media/WhatsAppLogo.svelte";
</script>

<header>
    <div class="header-container">
        <div class="logo-section">
            <a href="/" class="brand-link">Mauricio José Cárdenas </a>
        </div>

        <nav class="nav-menu">
            <a href="/">Inicio</a>
            <a href="/tutorias">Tutorías</a>
            <a href="/cursos">Cursos</a>
            <a href="/blog">Blog</a>
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
        background-color: #0c325a;
        border-bottom: 1px solid #2a2829;
        z-index: 1000;
    }

    .header-container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0.75rem 1.5rem;
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-between;
        gap: 2rem;
        align-items: center;
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

    .nav-menu a {
        color: #ffffff;
        font-weight: 500;
        /* font-size: 0.95rem; */
        text-decoration: none;
        transition: opacity 0.2s;
        white-space: nowrap;
    }

    .nav-menu a:hover {
        color: #ff7a00;
    }

    .social-icons {
        display: flex;
        align-items: center;
        gap: 1rem;
    }
</style>
