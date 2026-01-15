<script>
	// Navbar
</script>

<div class="sticky top-0 z-50 w-full bg-white">
	<!-- Top Banner -->
	<div class="bg-primary-900 px-4 py-2 text-center text-[11px] font-medium tracking-wide text-white">
		<a href="#" class="hover:underline uppercase tracking-[0.2em]">
			HiPeople is now SOC 2 Type II Certified &rarr; Learn More
		</a>
	</div>

	<!-- Main Navigation -->
	<nav class="border-b border-gray-100 px-6 py-4">
		<div class="mx-auto flex max-w-[1400px] items-center justify-between">
			<!-- Logo and Left Links -->
			<div class="flex items-center gap-12">
				<a href="/" class="text-xl font-bold tracking-tighter text-gray-900 flex items-center gap-2">
					<div class="w-6 h-6 bg-primary-600 rounded-sm"></div>
					HIPEOPLE
				</a>
				
				<div class="hidden items-center gap-8 md:flex">
					{#each ['Platform', 'Integrations', 'Customers', 'Resources'] as item}
						<a href="#" class="flex items-center gap-1 text-[11px] font-bold tracking-widest text-gray-500 hover:text-gray-900 uppercase">
							{item}
							{#if item === 'Platform' || item === 'Resources'}
								<svg width="10" height="10" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="opacity-50"><path d="m6 9 6 6 6-6"/></svg>
							{/if}
						</a>
					{/each}
				</div>
			</div>

			<!-- Right Actions -->
			<div class="flex items-center gap-6">
				<a href="#" class="text-[11px] font-bold tracking-widest text-gray-500 hover:text-gray-900 uppercase">
					Sign In
				</a>
				<a href="#" class="bg-gray-900 px-6 py-2.5 text-[11px] font-bold tracking-widest text-white transition-all hover:bg-primary-600 uppercase">
					Book a Demo
				</a>
			</div>
		</div>
	</nav>
</div>