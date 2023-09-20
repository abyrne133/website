<script>
	import Articles from '$lib/Articles.svelte';
	import bigOImage from '$lib/images/bigo.png';
	let articles = [
		{
			title: 'Big O Notation',
			description: 'Learn how to classify the efficiency of your algorightms with Big O Notation.',
			image: bigOImage,
			imageAlt: 'Big O Notation',
            link: 'big-o',
            buttonText: 'Show More'
		},
	];
</script>

<Articles {articles} />
