<script lang="ts">
	import type { Vault } from 'src/api/Vault';
import VaultListing from './VaultListing.svelte';

	export let vaults: Vault[];
</script>

<style>
	h1 {
		font-family: sans-serif;
	}

	h2 {
		font-family: sans-serif;
		font-weight: normal;
		color: #555;
	}
</style>

<h1>Crypton</h1>
<h2>Vaults</h2>
<hr>

{#each vaults as vault}
    <VaultListing {vault}/>
{/each}
