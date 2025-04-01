<script lang="ts">
	// [label,value]
	let values: [string, string][] = [
		['Light', 'light'],
		['Dark', 'dark'],
		['Abyss', 'abyss'],
		['Emerald', 'emerald'],
		['Cyberpunk', 'cyberpunk'],
		['Night', 'night'],
		['Sunset', 'sunset']
	];
</script>

<div class="dropdown">
	<div tabindex="0" role="button" class="btn m-1">Click</div>
	<ul class="dropdown-content menu bg-base-100 rounded-box z-1 w-52 p-2 shadow-sm">
		{#each values as [label, value]}
			<li>
				<input
					type="radio"
					name="theme-dropdown"
					class="theme-controller btn btn-sm btn-block btn-ghost justify-start"
					aria-label={label}
					{value}
				/>
			</li>
		{/each}
	</ul>
</div>
