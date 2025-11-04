<script lang="ts">
    // Simple Live Chat page — currently static text. Can be replaced to mount Chat component later.
</script>

<svelte:head>
    <title>Live Chat</title>
</svelte:head>

<div class="p-6">
    <h1 class="text-2xl font-semibold">{$i18n?.t ? $i18n.t('Live Chat') : 'Live Chat'}</h1>
    <p class="mt-3 text-gray-600">{$i18n?.t ? $i18n.t('Live Chat Tab Description') : 'これはLive Chat用のタブです'}</p>
</div>
