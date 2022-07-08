<script lang="ts">
	import type { Vault } from '../api/Vault';

	export let vault: Vault;
</script>

<h1>{vault.name}</h1>
<p>{vault.path}</p>
