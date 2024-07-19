<div class="flex w-full flex-col gap-12 px-12 pt-4">
	<h1 class="font-readex text-8xl font-black tracking-tighter text-white">Lead The Way</h1>
	<a href="/vote">
		<button class="button font-readex button--anthe relative bg-none px-16 py-4 text-white">
      <span class="block mix-blend-screen">Vote</span>
    </button>
	</a>
</div>

<style>
	.button::before,
	.button::after {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
	}

	.button--anthe::before {
		border-radius: 8px;
		content: '';
		background: linear-gradient(to right, var(--red), var(--purple));
		-webkit-clip-path: polygon(0% 0%, 100% 0, 100% 50%, 100% 100%, 0% 100%);
		clip-path: polygon(0% 0%, 100% 0, 100% 50%, 100% 100%, 0% 100%);
		transition:
			clip-path 0.4s cubic-bezier(0.2, 1, 0.8, 1),
			-webkit-clip-path 0.4s cubic-bezier(0.2, 1, 0.8, 1);
	}

	.button--anthe:hover::before {
		background: linear-gradient(to right, var(--red), var(--purple));
		-webkit-clip-path: polygon(0% 0%, 75% 0%, 100% 50%, 75% 100%, 0% 100%);
		clip-path: polygon(0% 0%, 75% 0%, 100% 50%, 75% 100%, 0% 100%);
	}

	.button--anthe span {
		transition: transform 0.4s cubic-bezier(0.2, 1, 0.8, 1);
	}

	.button--anthe:hover span {
		transform: translate3d(-10px, 0, 0);
	}
</style>
