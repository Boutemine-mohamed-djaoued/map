<script>
	import SearchBar from './SearchBar.svelte';
	import Info from './Info.svelte';
</script>

<header class="p-4 p-xl-5 position-relative ">
	<h1 class="mx-auto text-center text-light">IP Adress Tracker</h1>
	<SearchBar />
  <Info />
</header>

<style>
  * {
			font-family: 'Rubik', sans-serif;
  }
	header {
		box-sizing: border-box;
		background-size: cover;
		min-height: 20em;
	}
	@media (max-width: 576px) {
		header {
			background-image: url('../pattern-bg-mobile.png');
		}
	}

	@media (min-width: 577px) {
		header {
			background-image: url('../pattern-bg-desktop.png');
		}
	}

	@media (min-width: 1201px) {
	}
</style>
