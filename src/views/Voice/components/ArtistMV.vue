<template>
	<div class="mv">
		<List :list="mv.mvs"/>
	</div>
</template>

<script>
import {mapState} from "vuex"
export default {
	name: "mv",
	components:{
		List:()=>import("@/components/List")
	},
	computed:mapState('voice',['mv'])
};

</script>