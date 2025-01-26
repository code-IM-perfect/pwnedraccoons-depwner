<script>
	let { children, col = '', row = '' } = $props();
</script>

<button
	class="homeCard card border-[1px] border-surface-200-800 preset-filled-surface-100-900"
	style="grid-row:{row};grid-column:{col};"
>
	<div class="cardInner">
		{@render children()}
	</div>
</button>

<style>
	.homeCard {
		padding: min(5vh, 5vw);
		/* font-size: 2vh; */
	}
	.homeCard :global(.lucide-icon) {
		--icon-size: min(15vh, 12vw);
		height: var(--icon-size);
		width: var(--icon-size);
	}
</style>
