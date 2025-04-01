<script lang="ts">
	import { onNavigate } from '$app/navigation';
	import '../app.css';
	import Navbar from '../components/Navbar.svelte';

	let { children } = $props();
</script>

<Navbar />
{@render children()}
