<script lang="ts">
    import '../app.css'

    import Navbar from '$lib/components/Navbar.svelte'
    import Footer from '$lib/components/Footer.svelte'
</script>

<svelte:head>
    <title>Terra Tint</title>
    <meta name="description" content="Terra Tint">
    <meta property="og:locale" content="en_US" />
    <meta property="og:site_name" content="Terra Tint" />
    <meta property="og:title" content="Terra Tint | Eco-friendly Shirts" />
    <meta property="og:description" content="Fashionable Eco-friendly Shirts" />
    <meta property="og:type" content="website" />
    <meta property="og:url" content="https://www.terratint-tees.xyz/" />
    <meta property="og:image" content="https://www.terratint-tees.xyz/" />
    <meta property="article:publisher" content="https://www.terratint-tees.xyz/" />
    <meta name="twitter:card" content="summary_large_image" />
    <meta name="twitter:site" content="@terratint" />

    <script type="application/ld+json">
        {
            "@content": "http://schema.org",
            "@type": "WebPage",
            "@id": "https://www.terratint-tees.xyz/",
            "name": "Terra Tint | Eco-friendly Shirts",
            "url": "https://www.terratint-tees.xyz/",
            "image": "https://www.terratint-tees.xyz/"
        }
    </script>
</svelte:head>

<Navbar />
<slot />
<Footer />