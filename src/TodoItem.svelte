<script>
	import {createEventDispatcher} from 'svelte'
	
	const dispatch = createEventDispatcher()

	const removeTodo = () => {
		dispatch('remove', index)
	}

	export let todo;
	export let index;
</script>

<div class="ti">
	<span>{index + 1}: {todo}</span>
	<span class="ti__btn_del" on:click={removeTodo}>Удалить</span>
</div>


<style>
	.ti {
		display: inline-flex;
		justify-content: space-between;
		padding: 8px;
		background-color: steelblue;
		color: white;
	}
	.ti__btn_del {
		cursor: pointer;
	}
</style>