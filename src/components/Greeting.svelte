<script lang="ts">
  function randomMessage() {
    return messages[(Math.floor(Math.random() * messages.length))];
  }

  export let messages: string[] = [];
  let greeting: string = randomMessage();
</script>

<div>
  <h3>{greeting}! Thank you for visiting!</h3>
  <button on:click={() => {
    greeting = randomMessage();
  }}>
    New Greeting
  </button>
</div>
