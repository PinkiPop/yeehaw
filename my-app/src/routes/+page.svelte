<head>
<link rel="stylesheet" href="/src/routes/Soundboard.css">
</head>
<script>
	import Sbbutton from '../lib/sbbutton.svelte';
  let arr=[]
  for (let i = 1; i < 21; i++) {
    arr.push({name:`button${i}`, src:``})
  }
</script>
<!--<script src="/home/scarlat/projects/yeehaw/my-app/src/routes/addingsound/+page.js"></script>-->
<div class="Header">
  <h1>Best League of Legends Voice Lines</h1><br>
</div> 
{#each arr as item}
<Sbbutton name={item.name} audiosrc={item.src}></Sbbutton>
 {/each}


