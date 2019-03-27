<template>
	<div class="container">
		<div class="content"><router-view /></div>
		<div class="side-bar">
			<router-link to="/lib_exam">题库</router-link>
			<router-link to="/lib_resources">资源库</router-link>
			<router-link to="/lib_activity">活动库</router-link>
		</div>
		
	</div>
</template>

<script>
export default {
	name: 'Lib',
	data() {
		return {
			
		};
	}
};
</script>

<style scoped>
	.container{
		display: flex;
		width: 90%;
		margin: 0 auto;
	}
		
	.side-bar{
		display: flex;
		flex-direction: column;
		background-color: #fff;
		margin-top: 20px;
		margin-left: 20px;
		flex: 1 1 20%;
	}
	a{
		margin-top: 30px;
	}
	.content{
		flex: 1 1 80%;
		text-align:center;
		background-color: #fff;
		padding-bottom: 20px;
	}
</style>
