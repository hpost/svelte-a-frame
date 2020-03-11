<script>
  export let visible = true

  const handleClick = () => { visible = false }
</script>

{#if visible}
  <div class="splash">
    <div class="card">
      <h1>A-Frame Project</h1>
      <p>
        Move around using your keyboard (WASD keys) or by tapping the screen (mobile)
      </p>
      <button on:click={handleClick}>Enter</button>
    </div>
  </div>
{/if}

<style>
  .splash {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100vh;
    background-color: rgba(0, 0, 0, 0.7);
    z-index: 99999;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .card {
    max-width: 50%;
    background-color: #f1f1f1;
    text-align: center;
    padding: 3rem;
    border-radius: 1rem;
  }

  @media only screen and (max-width: 700px) {
    .card {
      max-width: 100%;
      border-radius: 0;
    }
  }

  button {
    margin-top: 1.5rem;
    padding: 1rem 1.5rem;
    border: none;
    background-color: black;
    color: white;
    cursor: pointer;
    font-size: 1.5em;
    text-transform: uppercase;
    font-weight: 700;
    border-radius: 0.5em;
  }
</style>