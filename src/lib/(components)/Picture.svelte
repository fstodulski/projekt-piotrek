<script lang="ts">
	export let product;

	console.log(product.title);
</script>

<div class="box">
	<img src={product.image} alt={product.title} />
</div>

<style>
	.box {
		display: flex;
		flex-direction: column;
		row-gap: 8px;
	}
</style>
