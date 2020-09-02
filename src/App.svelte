<script type="ts">
let name: string = "Alessandro"
let age: number = 20

$: uppercaseName = name.toUpperCase()

function incAge() {
	age += 1
}

function changeName() {
	name = "Max"
}
</script>


<h1>My name is {uppercaseName} and I am {age}</h1>
<button on:click="{incAge}">Click here to make me older</button>
<button on:click="{changeName}">Change Name</button>