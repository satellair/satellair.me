<script lang="ts">
  import Satella from "$lib/components/Satella.svelte"
</script>

<main class="flex flex-col justify-between w-screen h-screen bg-yellow-50 px-4 md:px-8">
	<div class="flex justify-between py-4">
		<div id="logo" class="">logo</div>
		<nav>
			<ul class="flex justify-between gap-8">
				<li class=""><a href="/">/project</a></li>
				<li class=""><a href="/">/card</a></li>
			</ul>
		</nav>
	</div>

	<section
		class="flex items-center justify-center border-[1px] border-black h-full w-full overflow-auto rounded-xl md:rounded-3xl"
	>
	 <Satella />
	</section>

	<section class="flex justify-end lg:justify-between py-4">
		<div class="hidden lg:block mt-4 max-w-[50%] text-sm xl:text-base pr-8 lg:pr-6">
			Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
			labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
			laboris nisi ut aliquip ex ea commodo consequat.
		</div>
		<h1 class="text-7xl lg:text-8xl xl:text-9xl font-bold">satellair.me</h1>
	</section>
</main>

<style>
</style>
