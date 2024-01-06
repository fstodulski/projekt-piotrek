<script lang="ts">
	import Picture from '$lib/(components)/Picture.svelte';

	type Product = {
		title: string;
		price: string;
		image: string;
	};

	type Database = Array<Product>;

	const database: Database = [
		{
			// 0
			title: 'Koza',
			price: '5$',
			image:
				'https://images.unsplash.com/photo-1682687221073-53ad74c2cad7?q=80&w=1770&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
		},
		{
			// 1
			title: 'stol',
			price: '10$',
			image:
				'https://images.unsplash.com/photo-1704241485844-5df18f026028?q=80&w=1315&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
		},
		{
			// 2
			title: 'kwiat',
			price: '15$',
			image:
				'https://plus.unsplash.com/premium_photo-1702742526094-74a4ad389d73?q=80&w=1287&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
		}
	];
</script>

{#each database as product}
	<Picture {product} />
{/each}
