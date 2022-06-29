<script>
  import Navbar from "./components/Navbar.svelte"
  import Title from "./components/Title.svelte"

  let fruits = ['apple', 'orange', 'lemon']

</script>

<main>
<Navbar />

<!-- DYNAMIC PROPS -->

<!-- <Title title="add expense" />
<Title title="expense list" /> -->

{#each fruits as fruitItem} 

<Title title={fruitItem}/>
<!-- <h1>Fruit: {fruitItem}</h1> -->

{/each}

</main>