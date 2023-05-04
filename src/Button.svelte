<svelte:options tag="my-button" />

<script>
import { onMount } from "svelte";
let data = []

    onMount(()=>{
      
	const fetch = async () => {
		const response = await fetch('https://jsonplaceholder.typicode.com/posts')
		const json = await response.json()
		console.log(json)
		data = json
	}
    fetch()
    })
   
</script>
<h1>Hello Sevlet</h1>
<h3>{data.length > 0 ? data[0].body : null}</h3>
<button class="btn">button</button>

<style>
.btn{
    background: blue;
}
</style>