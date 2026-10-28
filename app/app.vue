<script setup>
useHead({ htmlAttrs: { lang: "en" } });

useSeoMeta({
  title: "Aaron | LAMP Developer for WordPress and WooCommerce Plugins",
  description:
    "LAMP developer building WordPress and WooCommerce plugins: Mercado Pago PIX and Boleto payment gateway, S3 and Cloudflare R2 media migration, and a searchable reference library.",
  ogTitle: "Aaron | LAMP Developer for WordPress and WooCommerce Plugins",
  ogDescription:
    "WordPress and WooCommerce plugins, payment gateways and media tools, with live demos.",
  ogType: "website",
  ogUrl: "https://aaron18-portfolio.pages.dev/",
  twitterCard: "summary",
});

const siteUrl = "https://aaron18-portfolio.pages.dev/";

const schema = {
  "@context": "https://schema.org",
  "@graph": [
    {
      "@type": "WebSite",
      "@id": `${siteUrl}#website`,
      name: "Aaron | LAMP Developer",
      url: siteUrl,
      inLanguage: "en",
    },
    {
      "@type": "Person",
      "@id": `${siteUrl}#person`,
      name: "Aaron",
      url: siteUrl,
      jobTitle: "LAMP Developer",
      description:
        "LAMP developer building WordPress and WooCommerce plugins, payment gateways and media tools.",
      knowsAbout: [
        "PHP",
        "MySQL",
        "jQuery",
        "AJAX",
        "WordPress plugin development",
        "WooCommerce payment gateways",
      ],
      sameAs: ["https://github.com/aaronwsmith12"],
    },
  ],
};

useHead({
  script: [{ type: "application/ld+json", innerHTML: JSON.stringify(schema) }],
});

// Google Tag Manager, container GTM-N96CFK52
useHead({
  script: [
    {
      // innerHTML = the text placed inside the <script> tag.
      // This is Google's standard loader: it creates a new <script> that downloads gtm.js for our container.
      innerHTML: `(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
        new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
        j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
        'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
      })(window,document,'script','dataLayer','GTM-N96CFK52');`,
    },
  ],
  noscript: [
    {
      // tagPosition "bodyOpen" = put this right after <body> opens, which is where Google wants it.
      // It's a fallback for visitors who have JavaScript turned off.
      tagPosition: "bodyOpen",
      innerHTML: `<iframe src="https://www.googletagmanager.com/ns.html?id=GTM-N96CFK52" height="0" width="0" style="display:none;visibility:hidden"></iframe>`,
    },
  ],
});
</script>

<template>
  <main class="max-w-3xl mx-auto px-5 py-12">
    <header>
      <h1 class="text-5xl font-bold mb-2">Aaron</h1>
      <p class="text-muted text-lg">
        LAMP developer. I build WordPress and WooCommerce plugins, payment
        gateways and media tools.
      </p>
    </header>

    <section>
      <h2 class="text-2xl font-semibold mt-12 mb-4">Projects</h2>

      <article class="bg-card rounded-xl p-5 mb-4">
        <h3 class="text-xl font-semibold mb-1">
          Mercado Pago, PIX and Boleto gateway
        </h3>
        <p class="text-muted mb-3">
          WooCommerce payment gateway for Brazilian payments.
        </p>
        <p class="text-muted flex flex-wrap items-center gap-x-3">
          View on Upwork:
          <a
            class="text-accent hover:underline"
            href="https://www.upwork.com/services/product/development-it-a-fully-integrated-woocommerce-payment-gateway-for-mercado-pago-and-pix-2099642480893651729?ref=project_share"
            target="_blank"
            rel="noopener"
            >Starter</a
          >
          <a
            class="text-accent hover:underline"
            href="https://www.upwork.com/services/product/development-it-a-fully-integrated-woocommerce-payment-gateway-for-mercado-pago-and-pix-2099642480893651729?ref=project_share&tier=1"
            target="_blank"
            rel="noopener"
            >Standard</a
          >
          <a
            class="text-accent hover:underline"
            href="https://www.upwork.com/services/product/development-it-a-fully-integrated-woocommerce-payment-gateway-for-mercado-pago-and-pix-2099642480893651729?ref=project_share&tier=2"
            target="_blank"
            rel="noopener"
            >Advanced</a
          >
        </p>
      </article>

      <article class="bg-card rounded-xl p-5 mb-4">
        <h3 class="text-xl font-semibold mb-1">S3 / R2 media migration</h3>
        <p class="text-muted mb-3">
          Moves a WordPress media library to AWS S3 or Cloudflare R2.
        </p>
        <p class="text-muted flex flex-wrap items-center gap-x-3">
          View on Upwork:
          <a
            class="text-accent hover:underline"
            href="https://www.upwork.com/services/product/development-it-wordpress-media-offload-to-aws-s3-or-cloudflare-r2-2101162304431687333?ref=project_share"
            target="_blank"
            rel="noopener"
            >Starter</a
          >
          <a
            class="text-accent hover:underline"
            href="https://www.upwork.com/services/product/development-it-wordpress-media-offload-to-aws-s3-or-cloudflare-r2-2101162304431687333?ref=project_share&tier=1"
            target="_blank"
            rel="noopener"
            >Standard</a
          >
          <a
            class="text-accent hover:underline"
            href="https://www.upwork.com/services/product/development-it-wordpress-media-offload-to-aws-s3-or-cloudflare-r2-2101162304431687333?ref=project_share&tier=2"
            target="_blank"
            rel="noopener"
            >Advanced</a
          >
        </p>
      </article>

      <article class="bg-card rounded-xl p-5 mb-4">
        <h3 class="text-xl font-semibold mb-1">Reference Library plugin</h3>
        <p class="text-muted mb-3">
          Searchable reference library for WordPress, with custom post types,
          taxonomies and live AJAX search.
        </p>
        <p class="flex flex-wrap items-center gap-x-3">
          <a
            class="text-accent hover:underline"
            href="https://playground.wordpress.net/?blueprint-url=https://raw.githubusercontent.com/aaronwsmith12/reference-library/main/blueprint-demo.json"
            target="_blank"
            rel="noopener"
            >Open live demo</a
          >
          <a
            class="text-accent hover:underline"
            href="https://github.com/aaronwsmith12/reference-library"
            target="_blank"
            rel="noopener"
            >View on GitHub</a
          >
        </p>
      </article>

      <article class="bg-card rounded-xl p-5 mb-4">
        <h3 class="text-xl font-semibold mb-1">
          Block theme and worksheets demo
        </h3>
        <p class="text-muted mb-3">
          Hand-coded WordPress block theme with a live Playground demo.
        </p>
        <a
          class="text-accent hover:underline"
          href="https://playground.wordpress.net/?blueprint-url=https://raw.githubusercontent.com/aaronwsmith12/block-theme-portfolio/main/blueprint-live.json"
          target="_blank"
          rel="noopener"
          >Open demo</a
        >
      </article>
    </section>

    <footer class="mt-12 text-muted">
      <p class="mb-3">
        I'm a WordPress and WooCommerce developer. Each project above is a real,
        working plugin or theme that I built myself, so you can look at the code
        or try the live demos.
      </p>
    </footer>
  </main>
</template>
