<script>
	export let color;
	export let set_color;
</script>

<style>
	div {
		border-radius: 50%;
		width: 50px;
		height: 50px;
		margin: 10px;
	}

	div:hover {
		cursor: pointer;
	}

	.primary {
		background-color: var(--primary-color);
	}

	.secondary {
		background-color: var(--secondary-color);
	}

	.tertiary {
		background-color: var(--tertiary-color);
	}

	.quarnary {
		background-color: var(--quarnary-color);
	}
</style>

<div class="{color}" on:click="{() => set_color(color)}" />
