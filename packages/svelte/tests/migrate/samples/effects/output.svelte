<script>
	import { run } from 'svelte/legacy';

	let count = $state(0);
	run(() => {
		console.log(count);
	});
	run(() => {
		if (count > 10) {
			alert('too high')
		}
	});
	run(() => {
		console.log('foo');
		if (x) return;
		console.log('bar');
	});
	run(() => {
		$count = 1;
	});
	run(() => {
		foo.x = count;
	});
</script>

<button onclick={() => count++}>increment</button>