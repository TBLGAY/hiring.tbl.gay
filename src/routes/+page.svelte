<script>
  import IconButton from "$lib/LinkButton.svelte";
  import LinkButtonList from "$lib/LinkButtonList.svelte";
  import Navbar from "$lib/Navbar.svelte";
  import SplitContainer from "$lib/SplitContainer.svelte";
  import links_data from "$lib/assets/links.toml";

  const links = Object.values(links_data);
</script>

<svelte:head>
  <title>TBLGAY is Hiring!</title>
</svelte:head>

<SplitContainer>
  <div slot="left" class="left">
    <h1 style:font-family="'Signika Negative', sans-serif">TBLGAY is Hiring!</h1>
    <h3
      style:font-family="'DM Sans', sans-serif"
      style:font-size="1.196em"
      style:margin-bottom="0.1em"
    >
    help us run York University's 50+ year old queer service!
    </h3>
    <p
      style:font-family="'DM Sans', sans-serif"
      style:margin-top="0"
      style:font-size="1.1em"
    >
      we're hiring two members for our Internal Team, for the 2024 to 2025 term. get involved in running our daily operations, our design identity, our activism presence and more!
    </p>
  </div>
  <hr />
  <div slot="right" class="right">
    <LinkButtonList {links} />
  </div>
</SplitContainer>

<style>
  .left {
    height: 100%;

    display: flex;
    flex-direction: column;
    /* align-items: center; */
    justify-content: flex-start;
  }

  .left h1 {
    margin-top: 0.2em;
    color: rgb(66, 59, 59);
    font-size: 4em;
    margin-bottom: 0;
    text-shadow: 1px 1px 2px rgb(211, 173, 173);
  }


  :global(.wrapper) {
    align-items: center;
    display: flex;
    justify-content: center;
    height: 100%;
    width: 100%;
  }

  :global(body) {
    width: 100%;
    height: 100%;
  }
  
  :global(html) {
    width: 100%;
    height: 100%;
  }


</style>
