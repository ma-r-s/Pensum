<script>
	import '../app.pcss';
	import { ModeWatcher } from 'mode-watcher';
	import Toggle from '$lib/components/Toggle.svelte';
</script>

<ModeWatcher />
<article class="prose prose-sm dark:prose-invert container max-w-none p-10 py-10 sm:max-w-5xl">
	<div class="flex justify-between">
		<h1>Revision de carpeta</h1>
		<Toggle></Toggle>
	</div>
	<div class="flex justify-end gap-4">
		<a href="Vistas">Vistas</a>
		<a href="Reglas">Reglas</a>
		<a href="Pensum">Pensum</a>
		<a href="Lista">Lista</a>
	</div>
	<slot />
</article>
