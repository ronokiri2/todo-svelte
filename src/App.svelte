<script>
	import ToDoList from './ToDoList.svelte'
	let name = 'ghfhjgvjhfj';
</script>

<main>
	<h1>Hello {name}!</h1>
	<ToDoList/>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

</style>