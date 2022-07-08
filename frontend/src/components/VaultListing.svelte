<script lang="ts">
	import type { Vault } from '../api/Vault';

	export let vault: Vault;

	const onPathClick = (path: string) => {
		window.open("file://" + path)
	}
</script>

<style>
	h1 {
		font-family: sans-serif;
	}

	.path {
		font-family: monospace;
		color: #999;
		background-color: #262626;
		padding: 0.25em;
		border-radius: 0.25em;
		cursor: pointer;
	}
</style>

<div>
	<h1>{vault.name}</h1>
	<span class="path" on:click={_ => onPathClick(vault.path)}>{vault.path}</span>
</div>
