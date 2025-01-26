<script>
	import HomeButton from '../components/+HomeButton.svelte';

	import { ScanSearch, RefreshCcw } from 'lucide-svelte';

</script>

<svelte:head>
	<title>DePWNer</title>
</svelte:head>

<div class="dashContainer grid grid-cols-3 text-center">
	<HomeButton>
		<RefreshCcw />
		<h3>Run a Scan</h3>
	</HomeButton>
	<HomeButton>
		<ScanSearch />
		<h3>Statistics</h3>
	</HomeButton>
	<HomeButton>
		<ScanSearch />
		<h3>Run a Scan</h3>
	</HomeButton>
	<HomeButton>
		<ScanSearch />
		<h3>Run a Scan</h3>
	</HomeButton>
	<HomeButton col="3" row="1/3">
		<ScanSearch />
		<h3>Status</h3>
	</HomeButton>
</div>

<style>
	.dashContainer {
		gap: min(2vh, 2vw);
	}
</style>
