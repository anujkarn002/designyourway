<script>
	import SvelteTooltip from '../components/SvelteTooltip.svelte';
</script>

<svelte:head>
	<title>About</title>
</svelte:head>

<div class="flex justify-center">
	<div class="max-w-sm rounded overflow-visible shadow-lg h-100 my-4">
		<div class="px-6 py-4">
			<div class="font-bold text-xl mb-2">About DYW</div>
			<p class="text-gray-700 text-base">
				This template uses following technologies. </p>
		</div>
		<div class="px-6 py-4">
			<SvelteTooltip tip="Svelte is a tool for building fast web applications." top>
				<span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2">Svelte</span>
			</SvelteTooltip>
			<SvelteTooltip tip="Sapper is an application framework powered by Svelte." top>
				<span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2">Sapper</span>
			</SvelteTooltip>
			<SvelteTooltip tip="Tailwind CSS is a highly customizable, low-level CSS framework." top>
				<span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700">Tailwind CSS</span>
			</SvelteTooltip>
			<SvelteTooltip tip="Firebase Hosting is production-grade web content hosting for developers." top>
				<span class="inline-block bg-gray-200 rounded-full px-3 py-1 my-1 text-sm font-semibold text-gray-700">Firebase Hosting</span>
			</SvelteTooltip>
			<SvelteTooltip tip="Firebase Functions is a serverless framework that lets you automatically run backend code." top>
				<span class="inline-block bg-gray-200 rounded-full px-3 py-1 my-1 text-sm font-semibold text-gray-700">Firebase Functions</span>
			</SvelteTooltip>
		</div>
	</div>
</div>
