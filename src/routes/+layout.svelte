<script>
	import Layout from '../dashboard/Layout.svelte';
	// import Auth from '../authentication/Auth.svelte'
	// import { onMount } from 'svelte';

	// let hasSessionId = false;

	// onMount(async ()=>{
	// 	const sessionId = true;
	// 	hasSessionId = Boolean(sessionId);
	// })
</script>

<!-- {#if hasSessionId} -->
	<Layout>
		<slot />
	</Layout>
<!-- {:else}
<Auth />
{/if} -->
