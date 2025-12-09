<script>
	let name = $state('world');
	let count = $state(0);
</script>

<h1>Hello {name}!</h1>

<input bind:value={name} />
<button onclick={() => count += 1}>
	clicks: {count}
</button>

<div>
    <p>Notice the error in the Console tab of DevTools and notice how the button and the input bind doesn't work.</p>
    <blockquote>
        <p>The error should look like this:</p>
        <pre>
            Uncaught TypeError: Cannot read properties of undefined (reading 'start')
                at (index):82:26
        </pre>
    </blockquote>
</div>
