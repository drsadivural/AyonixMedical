<script>
	import { goto } from '$app/navigation';
	import { config } from '$lib/stores';
	import { onMount } from 'svelte';

	let loaded = false;

	onMount(async () => {
		if ($config) {
			await goto('/');
		}

		loaded = true;
	});
</script>

{#if loaded}
	<div class="absolute w-full h-full flex z-50">
		<div class="absolute rounded-xl w-full h-full backdrop-blur flex justify-center">
			<div class="m-auto pb-44 flex flex-col justify-center">
				<div class="max-w-md">
					<div class="text-center text-2xl font-medium z-50">Ayonix AI-MED Backend Required</div>

					<div class=" mt-4 text-center text-sm w-full">
						Oops! You're using an unsupported method (frontend only). Please serve the AI-MED from
						the backend.

						<br class=" " />
						<br class=" " />
						<a
							class=" font-semibold underline"
							href="http://gpt.ayonix.com"
							target="_blank">See readme.md for instructions</a
						>
						or
						<a class=" font-semibold underline" href="http://gpt.ayonix.com" target="_blank"
							>Go for help</a
						>
					</div>

					<div class=" mt-6 mx-auto relative group w-fit">
						<button
							class="relative z-20 flex px-5 py-2 rounded-full bg-gray-100 hover:bg-gray-200 transition font-medium text-sm"
							on:click={() => {
								location.href = '/';
							}}
						>
							Check Again
						</button>
					</div>
				</div>
			</div>
		</div>
	</div>
{/if}
