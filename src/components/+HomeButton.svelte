<script>
	let { children } = $props();
</script>

<button
	class="card grid place-items-center border-[1px] p-4 border-surface-200-800 preset-filled-surface-100-900"
>
	{@render children()}
</button>
