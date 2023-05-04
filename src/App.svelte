<script>
	export let name;
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>
	tristique senectus et netus et 
	malesuada fames ac turpis egestas. 
	Vestibulum tortor quam, feugiat vitae, 
	ultricies eget, tempor sit amet, ante. 
	Donec eu libero sit amet quam egestas semper. 
	Aenean ultricies mi vitae est. Mauris placerat eleifend leo.
	 Quisque sit amet est et sapien ullamcorper pharetra. 
	 Vestibulum erat wisi, condimentum sed, commodo vitae, ornare sit amet, wisi. Aenean fermentum, elit eget tincidunt condimentum, eros ipsum rutrum orci, sagittis tempus lacus enim ac dui. Donec non enim in turpis pulvinar facilisis. Ut felis. Praesent dapibus, neque id cursus faucibus, tortor neque egestas augue, eu vulputate magna eros eu erat. Aliquam erat volutpat. Nam dui mi, tincidunt quis, accumsan porttitor, facilisis luctus, metus</p>
</main>

<style>
	main {
		text-align: center;
		padding: 2em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 400;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>