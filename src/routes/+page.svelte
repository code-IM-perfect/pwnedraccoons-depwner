<script>
	import HomeButton from '../components/+HomeButton.svelte';

	import { ScanSearch } from 'lucide-svelte';
</script>

<div class="grid grid-flow-col text-center">
	<HomeButton>
		<ScanSearch />
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
</div>
