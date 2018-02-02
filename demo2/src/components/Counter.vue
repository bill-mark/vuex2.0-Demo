<template>
	<div>
		Count is {{ count}}
		<button @click="increment">+</button>
		<button @click="decrement">-</button>
	</div>
</template>
<script>
	import {mapGetters,mapActions} from 'vuex'
	export default {
		computed:mapGetters([
            'count'
		]),
		
		methods:mapActions([
			'increment',
			'decrement'
		])
	}
</script>