<script>
	//let fruits = ["Apple", "Banana", "Cherry", "Orange", "Mango"];
    
    //Props
    export let f;
</script>

<h2> 메뉴 리스트 </h2>

<ul>
    {#each f as fruit}
        <li>{fruit}</li>
    {/each}
</ul>
