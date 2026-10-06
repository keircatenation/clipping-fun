<script>
	import favicon from '#lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<style>
		body{
			margin: 0;
			padding: 0;
			font-family: Georgia, 'Times New Roman', Times, serif;
			--color--quantum-cobalt: #003EFF;
			--color--neon-green:#c7ff16;
			--color--urochester-navy:#001E5F;
			--color--wondrous-sky:#B7D3FF;
			--color--black:#000;
			--color--white: #fff;
			--color--charcoal-grey:#707070;
			--color--meridian-silver:#E8E8E8;
			--spacing--padding:clamp( var(--spacing--40), 7vw, var(--spacing--80) );
			--spacing--20:.75rem;
			--spacing--30:1.15rem;
			--spacing--40:1.5rem;
			--spacing--50:2rem;
			--spacing--60:3rem;
			--spacing--70:4.5rem;
			--spacing--80:6.75rem;
			--font-size--small:0.9rem;
			--font-size--normal:1.125rem;
			--font-size--medium:1.25rem;
			--font-size--medium-large:1.35rem;
			--font-size--large:clamp(1.55rem, 1.55rem + ((1vw - 0.2rem) * 0.563), 2rem);
			--font-size--x-large:clamp(1.7rem, 1.7rem + ((1vw - 0.2rem) * 0.875), 2.4rem);
			--font-size--xx-large:clamp(1.85rem, 1.85rem + ((1vw - 0.2rem) * 1.438), 3rem);
			--font-size--xxx-large:clamp(2rem, 2rem + ((1vw - 0.2rem) * 2.5), 4rem);
		}
		body * {
			box-sizing: border-box;
			font-size: var(--font-size--normal);
		}
	</style>
</svelte:head>

{@render children()}
