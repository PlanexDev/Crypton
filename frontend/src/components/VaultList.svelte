<script lang="ts">
	import type { Vault } from 'src/api/Vault';
import VaultListing from './VaultListing.svelte';

	export let vaults: Vault[];
</script>

<style>
	div {
		background-color: #101010;
		max-width: 1080px;
		margin: 2em auto;
		padding: 0 1em 1em 1em;
	}

	h1 {
		font-size: 3.5em;
		margin-bottom: 0;
		font-family: sans-serif;
	}
</style>

<div>
	<h1>Vaults</h1>
	<hr>
	
	{#each vaults as vault}
		<VaultListing {vault}/>
	{/each}
</div>
