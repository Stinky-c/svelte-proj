<script lang="ts">
	import AltThemeController from './AltThemeController.svelte';
</script>

<div class="navbar bg-base-200 shadow-sm">
	<div class="flex-1">
		<a class="btn btn-ghost text-3xl" href="/">daisyUI</a>
	</div>
	<div class="flex-1">
		<a class="btn btn-ghost text-xl" href="/docs">Docs</a>
	</div>

	<div class="flex-none">
		<button class="btn btn-square btn-ghost"> test </button>
	</div>
	<div class="flex-none">
		<AltThemeController />
	</div>
</div>
