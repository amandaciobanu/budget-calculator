<script>
  import Title from './Tittle.svelte';
  import Tittle from "./Tittle.svelte";
  let name = '';
  let amount = null;
</script>

<section class="form">
  <Tittle title="add expense" />
  <form class="expense-form">
    <div class="form-control">
      <label for="name">name</label>
      <input type="text" id="name" bind:value={name}>
    </div>
    <div class="form-control">
      <label for="amount">amount</label>
      <input type="number" id="amount" bind:value={amount}>
    </div>
    <p class="form-empty">Please fill out all fields</p>
    <button type="submit" class="btn btn-block">
      add expense
    </button>
    <button type="button" class="close-btn">
      <i class="fas fa-times"> </i>
      close
    </button>
  </form>
</section>