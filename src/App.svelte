<script>
  // components
  import Navbar from './components/Navbar.svelte'
  import ExpensesList from './components/ExpensesList.svelte'
  // data
  import expensesData from './expenses.js'
  //variables
  let expenses = [...expensesData]
  console.log(expenses)
</script>

<Navbar />
<main class="content">
  <!-- If prop and value names are the same, it often will auto-format from: 
    expenses="{expenses}" >>> TO >>> {expenses} -->
  <ExpensesList expenses="{expenses}" />
</main>
