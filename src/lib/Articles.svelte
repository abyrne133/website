<script>
	/**
	 * @type {import('./types').Article[]}
	 */
	export let articles;
</script>

<div class="grid">
	{#each articles as article}
		<article class="article">
			<header><strong>{article.title}</strong></header>
			<img class="article-image" src={article.image} alt={article.imageAlt} />
			<footer>
				<p>{article.description}</p>
				<a class="article-button" href={article.link} role="button">{article.buttonText}</a>
			</footer>
		</article>
	{/each}
</div>

<style>
	.article {
		cursor: pointer;
	}
	.article-image {
		height: auto;
		max-width: 100%;
	}
	.article-button {
		display: block;
	}
</style>
