<script>
	import * as Table from '$lib/components/ui/table';
	import { courseList } from '$lib/courseList.js';
</script>

<h2>Lista de clases</h2>
<Table.Root class="not-prose">
	<Table.Caption>Lista de tus materias vists.</Table.Caption>
	<Table.Header>
		<Table.Row>
			<Table.Head class="w-[100px]">Nombre</Table.Head>
			<Table.Head>Codigo</Table.Head>
			<Table.Head>Creditos</Table.Head>
			<Table.Head class="text-right">Atributos</Table.Head>
		</Table.Row>
	</Table.Header>
	<Table.Body>
		{#each courseList as course, i (i)}
			<Table.Row>
				<Table.Cell class="font-medium">{course.nombre}</Table.Cell>
				<Table.Cell>{course.codigo}</Table.Cell>
				<Table.Cell>{course.creditos}</Table.Cell>
				<Table.Cell class="text-right">{course.atributos}</Table.Cell>
			</Table.Row>
		{/each}
	</Table.Body>
</Table.Root>
