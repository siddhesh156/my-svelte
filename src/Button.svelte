<svelte:options tag="my-button" />

<script>
import { onMount } from "svelte";

    onMount(()=>{
        let data = []
	const fetchSomething = async () => {
		const response = await fetch('https://jsonplaceholder.typicode.com/posts')
		const json = await response.json()
		console.log(json)
		data = json
	}
    fetchSomething()
    })
   
</script>
<h1>Hello Sevlet</h1>
<button class="btn">my-button</button>

<style>
.btn{
    background: red;
}
</style>