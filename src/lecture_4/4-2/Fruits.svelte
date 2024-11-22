<script>
	//let fruits = ["Apple", "Banana", "Cherry", "Orange", "Mango"];
    
    //Props
    export let fruits;
    export let reverse;
    export let slice;

    let computedFruits = [];
    let title = "";

    if (reverse) {
        computedFruits = [...fruits].reverse(); 
        title = "메뉴 리스트 reverse";
    }
    else if (slice) {
        // slice => '-2'
        // slice => ['0'. '3']
        computedFruits = fruits.slice(...slice.split(','));
        title = `메뉴 리스트 slice ${slice}`;
    }
    else {
        computedFruits = fruits;
        title = "메뉴 리스트 ";
    }


</script>

<h2> {title} </h2>

<ul>
    {#each computedFruits as fruit}
        <li>{fruit}</li>
    {/each}
</ul>
