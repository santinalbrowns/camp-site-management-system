<aside class="p-6 w-72 absolute left-0 h-screen flex flex-col justify-between">
	<nav>
		<ul>
			<li>
				<a href="/admin">
					<span class="material-symbols-outlined"> insert_chart </span>
					<span>Dashboard</span>
				</a>
			</li>

			<li>
				<a href="/">
					<span class="material-symbols-outlined"> location_away </span>
					<span>Campsites</span>
				</a>
			</li>
			<li>
				<a href="/">
					<span class="material-symbols-outlined"> kitchen </span>
					<span>Resources</span>
				</a>
			</li>
			<li>
				<a href="/">
					<span class="material-symbols-outlined"> people </span>
					<span>Evacuees</span>
				</a>
			</li>
			<li>
				<a href="/">
					<span class="material-symbols-outlined"> favorite </span>
					<span>Donations</span>
				</a>
			</li>
		</ul>
	</nav>

	<form action="/logout" method="post" class="py-2">
		<button type="submit">Logout</button>
	</form>
</aside>

<main class="ml-72">
	<slot />
</main>

<style lang="postcss">
	nav ul li a {
		@apply flex px-2 py-1 items-center text-gray-800;
	}
	.material-symbols-outlined {
		font-variation-settings: 'FILL' 1, 'wght' 300, 'GRAD' 0, 'opsz' 24;
        @apply pr-3 text-yellow-500;
	}
</style>
