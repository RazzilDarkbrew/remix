<template>
	<Recommend :title="'推荐电台'" :to="'/broadcast-radio'" :list="dj" name="radio" />
</template>

<script>
import {mapState} from "vuex"
export default {
	components:{
		Recommend:()=>import("@/components/Recommend/index.vue")
	},
	name: "RecRadio",
	computed:mapState('home',['dj'])
};
</script>
