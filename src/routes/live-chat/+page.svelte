<script lang="ts">
	import Chat from '$lib/components/chat/Chat.svelte';
	import { WEBUI_NAME } from '$lib/stores';
</script>

<svelte:head>
	<title>{`${$WEBUI_NAME ?? 'Open WebUI'} | Live Chat`}</title>
</svelte:head>

<div class="h-full w-full flex flex-col">
	<h1 class="sr-only">Live Chat</h1>
	<Chat />
</div>
