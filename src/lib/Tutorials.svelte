<script>
	import Articles from '$lib/Articles.svelte';
	import bigOImage from '$lib/images/bigo.png';
	import hashTablesImage from '$lib/images/hash-table.png';
	let articles = [
		{
			title: 'Big O Notation',
			description: 'Learn how to classify the efficiency of your algorightms with Big O Notation.',
			image: bigOImage,
			imageCaption: 'The letter O with code in the background sort of like hyper space to represent big o notation.',
			imageAlt: 'Big O Notation',
            link: 'big-o',
            buttonText: 'Show More'
		},
		{
			title: 'Hash Tables',
			description: 'The data strcuture thats used everywhere, learn about hashing and collisions.',
			image: hashTablesImage,
			imageCaption: 'Data table from computing with cartoon like symbols like batman and rick astley.',
			imageAlt: 'Hash Tables',
            link: 'hash-tables',
            buttonText: 'Show More'
		},
		
	];
</script>

<p>AI generated images are used because let's follow the hype, the description used to generate each image is provided in the captions - for the excitement.</p>
<Articles {articles} />
