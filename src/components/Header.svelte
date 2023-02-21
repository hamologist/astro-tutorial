<script lang="ts">
  import Hamburger from "./Hamburger.svelte";
  import Navigation from "./Navigation.svelte";

  let expanded: boolean = false;
</script>

<nav>
  <Hamburger onClick={() => {
    expanded = !expanded;
  }}/>
  <Navigation expanded={expanded}/>
</nav>
