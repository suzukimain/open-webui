<script lang="ts">
	// Live2D 表示用のプレースホルダコンポーネント
	// 実際の Live2D ランタイム（pixi.js + live2d.js 等）を組み込む場合はここに初期化コードを追加してください。
	import { onMount, onDestroy } from 'svelte';
	let container: HTMLDivElement | null = null;

	onMount(() => {
		// ここで Live2D を初期化
		console.log('Live2D mount');
	});

	onDestroy(() => {
		// クリーンアップ
		console.log('Live2D destroy');
	});
</script>

<style>
	.live2d-placeholder {
		width: 100%;
		height: 100%;
		display: flex;
		align-items: center;
		justify-content: center;
		background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(0,0,0,0.02));
		border-radius: 8px;
	}
</style>

<div bind:this={container} class="live2d-placeholder">
	<div class="text-center text-sm text-gray-600 dark:text-gray-400">
		Live2D area
		<div class="text-xs mt-1 text-gray-400">ここに Live2D 表示を実装してください</div>
	</div>
</div>
