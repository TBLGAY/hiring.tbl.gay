<script lang="ts">
  import "$lib/assets/styles/fonts.css";

  import IconButton from "$lib/LinkButton.svelte";
  import LinkButtonList from "$lib/LinkButtonList.svelte";
  import Navbar from "$lib/Navbar.svelte";
  // import Discord from

  const links = [
    {
      name: "home",
      href: "/",
    },
    {
      name: "about",
      href: "/about",
    },
    {
      name: "drop-in",
      href: "/space",
    },
    {
      name: "resources",
      href: "/resources",
    },
    // {
    //     "name": "Drop-in Space",
    //     "href": "/space",
    //     "icon": "mdi:location",
    //     "color": "white",
    //     "background": "#647d6a"
    // }
  ];
</script>

<svelte:head>
  <meta
    name="description"
    content="come help us run YorkU's 50+ year old queer service group"
  />

  <!-- Facebook Meta Tags -->
  <meta property="og:url" content="https://hiring.tbl.gay" />
  <meta property="og:type" content="website" />
  <meta property="og:title" content="TBLGAY is hiring!" />
  <meta
    property="og:description"
    content="come help us run YorkU's 50+ year old queer service group"
  />
  <meta property="og:image" content="https://hiring.tbl.gay/cover.jpg" />

  <!-- Twitter Meta Tags -->
  <meta name="twitter:card" content="summary_large_image" />
  <meta property="twitter:domain" content="hiring.tbl.gay" />
  <meta property="twitter:url" content="https://hiring.tbl.gay" />
  <meta name="twitter:title" content="TBLGAY is hiring!" />
  <meta
    name="twitter:description"
    content="come help us run YorkU's 50+ year old queer service group"
  />
  <meta name="twitter:image" content="https://hiring.tbl.gay/cover.jpg" />

  <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png" />
  <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png" />
  <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png" />
  <link rel="manifest" href="/site.webmanifest" />

  <script async src="https://umami.cat-girl.gay/script.js" data-website-id="25038b8d-7b3b-46d1-a1c0-16a61e78c18f"></script>
</svelte:head>

<!-- <Navbar {links} />

<hr class="nav-separator" /> -->

<slot />

<style>

</style>
