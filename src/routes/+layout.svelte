<script lang="ts">
	import '../app.css';
	let { children } = $props();

	import { Navigation } from '@skeletonlabs/skeleton-svelte';
	import { Settings, House, Logs, ChartNoAxesColumn, ChartSpline } from 'lucide-svelte';
</script>

<div class="cont flex h-[100vh]">
	<Navigation.Rail>
		{#snippet header()}
			<div
				class="icon flex aspect-square w-full flex-col items-center justify-center gap-1 rounded-container p-2 hover:preset-filled-surface-50-950"
			>
				DePWN
			</div>
		{/snippet}
		{#snippet tiles()}
			<Navigation.Tile id="0" label="Dash" href="/" labelExpanded="Dashboard">
				<House />
			</Navigation.Tile>
			<Navigation.Tile id="1" label="Logs" href="/logs" labelExpanded="Scan Logs">
				<Logs />
			</Navigation.Tile>
			<Navigation.Tile id="2" label="Stats" href="/stats" labelExpanded="Statistics">
				<ChartSpline />
			</Navigation.Tile>
			<Navigation.Tile id="3" label="Schedule" href="/schedule" labelExpanded="Schedule">
				<CalendarDays />
			</Navigation.Tile>
		{/snippet}
		{#snippet footer()}
			<Navigation.Tile labelExpanded="Settings" href="/settings" title="settings">
				<Settings />
			</Navigation.Tile>
		{/snippet}
	</Navigation.Rail>
	<main class="cont grid h-[100vh] w-full place-items-center">
		{@render children()}
	</main>
</div>
