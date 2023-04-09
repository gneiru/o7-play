<script lang="ts">
	import { trpc } from '$lib/trpc';

	const res = trpc.greeting.query({ name: 'gneiru' });
</script>

<h1>{$res.data}</h1>