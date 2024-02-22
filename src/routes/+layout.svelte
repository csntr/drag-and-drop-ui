<script>
	import '../app.css';
</script>

<div class="layout-grid">
	<nav class="header dark:bg-gray-900">Header</nav>
	<main class="content">
		<slot />
	</main>
</div>

<style>
	.layout-grid {
		display: grid;
		grid-template-areas:
			'header'
			'content';
    grid-template-rows: 4rem auto;
	}

	.header {
		grid-area: header;
	}

	.content {
		grid-area: content;
	}
</style>
