<script lang="ts">
	import { page } from "$app/state";
</script>

<main class="min-h-screen flex flex-col items-center justify-center px-6 bg-white text-black">
	<div class="max-w-md text-center">
		<svg width="64" height="40" viewBox="0 0 102 64" fill="none" xmlns="http://www.w3.org/2000/svg" class="mx-auto mb-8 opacity-50">
			<path fill-rule="evenodd" clip-rule="evenodd" d="M0.464844 36.6203C20.766 36.6203 37.2233 20.2248 37.2233 0H64.7063C64.7063 20.2248 81.1637 36.6203 101.465 36.6203V64C80.9762 64 62.7279 54.4446 50.9648 39.563C39.2018 54.4446 20.9534 64 0.464844 64V36.6203Z" fill="black"/>
		</svg>
		<h1 class="text-6xl font-bold mb-4">{page.status}</h1>
		<p class="text-lg text-gray-600 mb-8">{page.error?.message ?? "Something went wrong."}</p>
		<a href="/" class="inline-block bg-black text-white px-8 py-3 rounded-full text-sm font-bold uppercase tracking-wide hover:bg-gray-800 transition-colors">
			Return Home
		</a>
	</div>
</main>
