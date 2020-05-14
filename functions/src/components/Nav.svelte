<script>
	export let segment;
	let navbar = {toggle: false};

	function toggleNavbar() {
		navbar.toggle = !navbar.toggle;
	}
</script>

<style>
	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		width: calc(100% - 2em);
		height: 2px;
		background-color: rgb(255, 62, 0);
		display: block;
		bottom: -1px;
	}
</style>

<nav class="sticky top-0">
	<div class=" container mx-auto px-6 py-2 flex flex-col sm:flex-row w-full justify-between items-center">
		<div class="w-full sm:w-auto self-end sm:self-center flex flex-row sm:flex-none flex-no-wrap justify-between items-center ">
			<a class="font-bold text-2xl lg:text-4xl py-1" href=".">
				DYW
			</a>
			<div class="block lg:hidden">
				<button on:click={toggleNavbar} class="flex items-center px-3 py-2 border rounded text-gray-500 border-gray-600 hover:text-gray-800 hover:border-teal-500 appearance-none focus:outline-none">
					<svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
						<title>Menu</title>
						<path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
					</svg>
				</button>
			</div>
		</div>

		<div class='{!navbar.toggle? "hidden": ""} sm:flex-row lg:block'>
			<ul class="inline-flex">
				<li><a class="px-4 hover:text-gray-800" aria-current='{segment === "undefined" ? "page" : undefined}' href='.'>Home</a></li>
				<li><a class="px-4 hover:text-gray-800" aria-current='{segment === "blog" ? "page" : undefined}' href='blog'>Blog</a></li>
				<li><a class="px-4 hover:text-gray-800" aria-current='{segment === "about" ? "page" : undefined}' href='about'>About</a></li>
				<li><a class="px-4 hover:text-gray-800" rel=prefetch aria-current='{segment === "contact" ? "page" : undefined}' href='contact'>Contact</a></li>
			</ul>
		</div>
	</div>
</nav>
