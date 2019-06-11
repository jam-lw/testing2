<script>
	import Container from "./Container.svelte";
	import Header from "./Header.svelte";
	import { Items, Item } from "./items";

	export let name = "Potato";
	export let header_color = "secondary";

	const set_header_color = new_color => header_color = new_color;
</script>

<style>
	:global(:root) {
		--background-color: #f9eed9;
		--primary-color: #49849b;
		--secondary-color: #fc7a66;
		--tertiary-color: #ffc67b;
		--quarnary-color: #18a5a5;
	}

	:global(body) {
		background-color: var(--background-color);
		color: var(--primary-color);
		font-family: ProximaNova, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
		margin: 0;
		padding: 0;
	}
</style>

<Container>
	<Header color={header_color}>Hello there Mr. {name}</Header>
	<Items>
		<Item color="primary" set_color={set_header_color} />
		<Item color="secondary" set_color={set_header_color} />
		<Item color="tertiary" set_color={set_header_color} />
		<Item color="quarnary" set_color={set_header_color} />
	</Items>
</Container>
