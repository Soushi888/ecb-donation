<script lang="ts">
	export let amount: number | null = null;
</script>

<div>
	<a
		class="btn variant-filled-primary hover:variant-filled-primary w-full"
		href="https://mixpay.me/ecole/{amount ? `${amount}usd` : ''}"
		target="_blank"
	>
		{#if !amount}
			Choose Amount
		{:else}
			{amount} $US
		{/if}
	</a>
</div>
