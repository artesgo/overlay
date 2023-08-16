<script lang="ts">
  import './app.scss';

	import { Bottom, Top } from '$lib';
</script>

<main>
	<div class="top"><Top /></div>
	<div class="content"></div>
	<div class="bottom"><Bottom /></div>
</main>

<style>
	main {
		display: grid;
		grid-template-columns: 10px 340px 20px 1fr 10px;
		grid-template-rows: 50px 1fr 80px;
		height: 100vh;
		overflow: hidden;
    background: #333;
	}

	.top {
		grid-column-start: 1;
		grid-column-end: 5;
		text-align: center;
	}

	.content {
		background: #00ff00;
		border-radius: 24px;
    box-shadow: inset 0px 0px 8px #333;
		grid-column-start: 2;
		grid-column-end: 5;
	}

	.bottom {
		grid-column-start: 1;
		grid-column-end: 5;
	}
</style>
