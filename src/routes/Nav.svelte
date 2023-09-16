<script>
	import Fa from 'svelte-fa';
	import { faBars } from '@fortawesome/free-solid-svg-icons';
</script>

<nav>
	<ul>
		<li>
			<hgroup>
				<h1 class="primary">Hello Dev</h1>
				<h6><mark>Now Learn.</mark></h6>
			</hgroup>
		</li>
	</ul>
	<ul class="menu">
		<li ><Fa icon={faBars} /></li>
	</ul>
</nav>

<style>
    .menu {
        font-size: 32px;
        align-items: flex-start;
    }
</style>
