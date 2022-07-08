<script lang="ts">
    import "../global.css"
	import type { Vault } from 'src/api/Vault';

	import VaultList from '../components/VaultList.svelte';

	const vaults: Vault[] = [
		{
			name: 'My Secret Information',
			path: '/home/user/vaults/secret_information',
			favorited: true
		},
		{
			name: 'Plans For World Domination',
			path: '/home/user/vaults/world_plans',
			favorited: false
		}
	];
</script>

<VaultList {vaults} />
