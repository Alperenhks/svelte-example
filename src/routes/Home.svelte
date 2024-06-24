<script>
  import { count } from "../store.js";
  const message = "Ana Sayfa";
  function increment() {
    count.update((n) => n + 1);
  }
</script>

<div class="home-container">
  <h1>{message}</h1>
  <p>Butona tıkladınız {$count} .</p>
  <button on:click={increment}>Arttır</button>
</div>

<style>
  .home-container {
    text-align: center;
    padding: 2em;
    font-family: Arial, sans-serif;
  }

  h1 {
    color: #333;
  }

  button {
    padding: 0.5em 1em;
    font-size: 1rem;
    margin-top: 1em;
    cursor: pointer;
  }
</style>
