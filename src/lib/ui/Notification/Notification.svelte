<script lang="ts">
	import type { Snippet } from 'svelte';

	interface Props {
		styles: {
			container: string;
		};
		title?: Snippet;
		content?: Snippet;
		footer?: Snippet;
	}

	let { styles, title, content, footer }: Props = $props();

	let isOpen = $state(false);
</script>

<div class={styles.container}>
	{#if title}
		{@render title()}
	{/if}

	{#if content}
		{@render content()}
	{/if}

	{#if footer}
		{@render footer()}
	{/if}
</div>
