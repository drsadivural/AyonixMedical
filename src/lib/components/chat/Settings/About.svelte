<script lang="ts">
	import { getOllamaVersion } from '$lib/apis/ollama';
	import { WEBUI_NAME, WEB_UI_VERSION } from '$lib/constants';
	import { config } from '$lib/stores';
	import { onMount } from 'svelte';

	let ollamaVersion = '';
	onMount(async () => {
		ollamaVersion = await getOllamaVersion(localStorage.token).catch((error) => {
			return '';
		});
	});
</script>

<div class="flex flex-col h-full justify-between space-y-3 text-sm mb-6">
	<div class=" space-y-3">
		<div>
			<div class=" mb-2.5 text-sm font-medium">{WEBUI_NAME} app version</div>
			<div class="flex w-full">
				<div class="flex-1 text-xs text-gray-700 dark:text-gray-200">
					{$config && $config.version ? $config.version : WEB_UI_VERSION}
				</div>
			</div>
		</div>

		<hr class=" dark:border-gray-700" />

		<div>
			<div class=" mb-2.5 text-sm font-medium">AI-MED LLM version</div>
			<div class="flex w-full">
				<div class="flex-1 text-xs text-gray-700 dark:text-gray-200">
					{ollamaVersion ?? 'N/A'}
				</div>
			</div>
		</div>

		<hr class=" dark:border-gray-700" />

		<div class="flex space-x-1">
			<a href="https://discord.gg/5rJgQTnV4s" target="_blank">
				<img
					alt="Ayonix Pty ltd"
					src="https://img.shields.io/badge/Linkedin-Ayonix%20AI%20MED-blue?logo=linkedin&logoColor=white"
				/>
			</a>

		</div>

		<div class="mt-2 text-xs text-gray-400 dark:text-gray-500">
			Developed by <a
				class=" text-gray-500 dark:text-gray-300 font-medium"
				href="https://ayonix.com"
				target="_blank">Ayonix Pty Ltd, AI Center, Australia</a
			>
		</div>
	</div>
</div>
