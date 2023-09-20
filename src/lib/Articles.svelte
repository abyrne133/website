<script>
	/**
	 * @type {import('./types').Article[]}
	 */
	export let articles;
</script>

<div class="articles">
	{#each articles as article}
		<article>
			<header><strong>{article.title}</strong>
			</header>
			<figure>
				<img class="article-image" src={article.image} alt={article.imageAlt} />
				<figcaption class="caption">{article.imageCaption}</figcaption>
			</figure>
			<footer>
				<p>{article.description}</p>
				<a class="article-button" href={article.link} role="button">{article.buttonText}</a>
			</footer>
		</article>
	{/each}
</div>

<style>
	.articles {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
		gap: 1rem;
	}

	.article-image {
		height: auto;
		max-width: 100%;
	}
	.caption{
		font-size: 0.8rem;
		font-style: italic;
		text-align: justify;
	}
	.article-button {
		display: block;
	}
</style>
