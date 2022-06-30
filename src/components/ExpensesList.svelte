<script>
  import SectionTitle from './Title.svelte'
  import SingleExpense from './SingleExpense.svelte'
  export let expenses = []
</script>

<style>
  h2 {
    text-transform: capitalize;
  }
</style>

<section>
  <SectionTitle title="Expense List" />
  <ul>
    {#each expenses as expense, index}
    <SingleExpense index="{index + 1}" />
    {:else}
    <h2>Currently you have no expenses</h2>
    {/each}
  </ul>
</section>
