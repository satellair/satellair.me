<script>
	import './tailwind.css';
	import { dev } from '$app/environment';
	import { inject } from '@vercel/analytics';
 
	inject({ mode: dev ? 'development' : 'production' });
</script>

<main class="flex flex-col w-screen h-screen bg-yellow-50 px-4 md:px-8">
	<div class="flex justify-between py-4">
		<div id="logo" class="relative block">
			<a href="/" aria-label="back_2_home">
				<img
					class="w-8 items-center aspect-square rounded-full"
					src="https://github.com/satellair.png"
					alt="profile_icon"
				/>
			</a>
		</div>
		<nav>
			<ul class="flex justify-between gap-8">
				{#each ['/project', '/card'] as item}
					<a href={item} class="group">
						<li
							class="bg-left-bottom bg-gradient-to-r from-gray-700 to-gray-900 bg-[length:0%_2px] bg-no-repeat group-hover:bg-[length:100%_2px] transition-all duration-200 ease-out"
						>
							{item}
						</li>
					</a>
				{/each}
			</ul>
		</nav>
	</div>
	<slot />
</main>
