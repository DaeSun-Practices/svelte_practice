<script>
	import Fruits from "./Fruits.svelte";
	let fruits = ["Apple", "Banana", "Cherry", "Orange", "Mango"];

</script>


<body> 
	<h1> 공무직근로자 급여관리체계 재개발 </h1>
	
	<!-- props의 이름과 변수명이 같으면 생략이 가능하다. -->
	<Fruits {fruits}/>
	<Fruits {fruits} reverse={true}/>
	<Fruits {fruits} slice = "-2"/>
	<Fruits {fruits} slice = "0, 3"/>


</body>
