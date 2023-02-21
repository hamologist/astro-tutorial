<style>
  div {
    padding-right: 20px;
    cursor: pointer;
    display: block;
  }

  div span {
    display: block;
    width: 40px;
    height: 5px;
    margin-bottom: 10px;
    background-color: #ff9776;
  }

  @media screen and (min-width: 636px) {
    div {
      display: none;
    }
  }
</style>

<script lang="ts">
  export let onClick: () => void;
</script>

<div on:click={onClick} on:keypress={onClick}>
  <span />
  <span />
  <span />
</div>
