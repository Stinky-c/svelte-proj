<script lang="ts">
	let { github_profile, alt = "Author's avatar" } = $props();
</script>

<div class="avatar">
	<div class="w-12 rounded-full">
		<img src="https://github.com/{github_profile}.png" {alt} />
	</div>
</div>
