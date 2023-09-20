<script>
	import Articles from '$lib/Articles.svelte';
	import bigOImage from '$lib/images/bigo.png';
	import hashTablesImage from '$lib/images/hash-table.png';
	let articles = [
		{
			title: 'Big O Notation',
			description: 'Learn how to classify the efficiency of your algorightms with Big O Notation.',
			image: bigOImage,
			imageCaption: 'AI Prompt: "The letter O with code in the background sort of like hyper space to represent big o notation."',
			imageAlt: 'Big O Notation',
            link: 'big-o',
            buttonText: 'Show More'
		},
		{
			title: 'Hash Tables',
			description: "The data strcuture that's used everywhere, learn about hashing and collisions.",
			image: hashTablesImage,
			imageCaption: 'AI Prompt: "Data table from computing with cartoon like symbols like batman and rick astley."',
			imageAlt: 'Hash Tables',
            link: 'hash-tables',
            buttonText: 'Show More'
		},
		
	];
</script>
<Articles {articles} />
