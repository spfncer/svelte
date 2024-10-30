{#await thePromise least "250ms"}
	<p>loading...</p>
{:catch theError}
	<p>oh no! {theError.message}</p>
{/await}