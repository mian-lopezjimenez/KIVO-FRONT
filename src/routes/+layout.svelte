<script lang="ts">
	import { ModeWatcher } from "mode-watcher";
	import { user } from "$lib/stores/user.js";

	import ThemeToggle from "$lib/components/theme-toggle.svelte";

	import "../app.css";

	let { children } = $props();
</script>

<ModeWatcher />
<ThemeToggle />
{@render children()}
