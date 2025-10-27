<script>
	import Notification from '../Notification/Notification.svelte';
</script>

{#snippet title()}
	<h2 class="text-base font-semibold">We use cookies</h2>
{/snippet}

{#snippet content()}
	<p class="pt-2 text-sm font-normal text-neutral-600">
		We use cookies to enhance your browsing experience and improve our website's performance. By
		continuing to use this site, you consent to the use of cookies. To learn more about how we use
		cookies and your options, please read our <a
			href="#"
			class="text-blue-600 underline hover:text-blue-800">cookie policy</a
		>.
	</p>
{/snippet}

{#snippet footer()}
	<div class="mt-auto flex items-center justify-between gap-4 self-stretch">
		<button class="mr-auto rounded bg-red-600 px-3.5 py-2.5 text-white">Decline all</button>
		<button class="rounded bg-indigo-700 px-4 py-2.5 text-white">Allow cookies</button>
		<button class="rounded border-[0.5px] border-solid border-neutral-200 bg-white px-4 py-2.5"
			>Manage cookies</button
		>
	</div>
{/snippet}

<Notification
	styles={{
		container: 'flex flex-col w-full h-50 p-4 md:py-6 md:px-8 lg:px-28 bottom-0 bg-white absolute'
	}}
	{title}
	{content}
	{footer}
/>
