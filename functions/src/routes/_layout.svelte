<script>
	import Nav from '../components/Nav.svelte';
	import Footer from '../components/Footer.svelte';

	export let segment;
</script>


<Nav {segment}/>

<main class="flex-1 mx-auto mb-auto">
	<slot></slot>
</main>

<Footer />
