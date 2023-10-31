<script>
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
</script>

<Navbar let:hidden let:toggle>
	<NavBrand href="/">
		<img
			src="https://placehold.co/600x300"
			class="mr-3 h-6 sm:h-9"
			alt="remix-ts-flowbite-starter"
		/>
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
			remix-ts-flowbite-starter
		</span>
	</NavBrand>
	<NavHamburger on:click={toggle} />
	<NavUl {hidden}>
		<NavLi href="/" active={true}>Home</NavLi>
	</NavUl>
</Navbar>
