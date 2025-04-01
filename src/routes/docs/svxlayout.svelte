<script lang="ts">
	import Avatar from '../../components/Avatar.svelte';
	import type { LayoutProps } from './$types';
	let {
		children,
		title,
		published,
		updated,
		author,
		github = 'stinky-c',
		hidden = false
	}: {
		title: String;
		published: String;
		updated: String;
		author: String;
		github: String;
		hidden: boolean;
	} & LayoutProps = $props();
</script>

<h1>{title}</h1>
<p class="date">Published on: {published}</p>
<p class="date">Updated at: {updated}</p>
<div>
	<p>By: {author}</p>
	<Avatar github_profile={github} />
</div>
{@render children()}
