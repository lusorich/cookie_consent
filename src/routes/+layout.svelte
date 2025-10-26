<script>
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

{@render children?.()}

<div class="credits" data-gfe-screenshot-exclude="true">
	A challenge by
	<a
		href="https://www.greatfrontend.com/projects?ref=challenges"
		target="_blank"
		rel="noopener noreferrer"
	>
		GreatFrontEnd Projects
	</a>. Built by
	<a
		href="https://www.greatfrontend.com/projects/u/dreamonautre"
		target="_blank"
		rel="noopener noreferrer"
	>
		dreamonaut
	</a>.
</div>
