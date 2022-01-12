<svelte:options tag="my-button" />

<script>
import { onMount } from "svelte";
let data = []

    onMount(()=>{
      
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
<h3>{data.length > 0 ? data[0].body : null}</h3>
<button class="btn">my-button</button>

<style>
.btn{
    background: red;
}
</style>