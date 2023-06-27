<script lang="ts">
	import { AppBar, Avatar } from '@skeletonlabs/skeleton';
</script>

<AppBar gridColumns="grid-cols-1" slotLead="place-self-center gap-3">
	<svelte:fragment slot="lead">
		<a href="https://www.ecoleduconsensusblockchain.com" target="_blank">
			<img
				src="logo_ecoleconsensusblockchain.png"
				alt="Logo Ecole Consensus Blockchain"
				class="h-52 rounded-lg"
			/>
		</a>
	</svelte:fragment>
</AppBar>
