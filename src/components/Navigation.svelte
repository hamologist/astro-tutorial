<style>
  div a {
    text-align: center;
    padding: 10px 0;
    text-decoration: none;
    font-size: 1.2rem;
    font-weight: bold;
    text-transform: uppercase;
  }

  .dark div a {
    color: #fff;
  }

  div a:hover, a:focus {
    background-color: #ff9776;
  }

  @media screen and (min-width: 636px) {
    div {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
      grid-gap: 1rem;
      margin: 0;
    }

    div a {
      padding: 15px 20px;
    }
  }

  @media screen and (max-width: 636px) {
    div {
      display: none;
      grid-template-rows: 1fr 1fr 1fr 1fr 1fr;
      grid-gap: 1rem;
      margin: 0;
    }
  }

  .expanded {
    display: grid;
  }
</style>

<script lang="ts">
    import ThemeIcon from "./ThemeIcon.svelte";


  export let expanded: boolean;
</script>

<div class:expanded={expanded}>
  <a href="/">Home</a>
  <a href="/about">About</a>
  <a href="/blog">Blog</a>
  <a href="/tags">Tags</a>
  <ThemeIcon />
</div>
