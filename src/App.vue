<template>
	<div class="container-fluid">
		<div class="row">
			<div class="col-md-12 init">
				<img alt="Vue logo" src="./assets/bc.webp" style="width: 150px" />
			</div>
			<div class="col-md-12 init">
				<skills msg="Welcome to My Portfolio App" />
			</div>
			<div class="col-md-12">
				<separator />
			</div>
			<div class="col-md-12">
				<blog />
			</div>
		</div>
	</div>
</template>

<script>
import skills from "./components/skills.vue";
import blog from "./components/blog.vue";
import separator from "./components/separator.vue";

export default {
	name: "App",
	components: {
		skills,
		blog,
		separator
	},
};
</script>

<style>
.init {
	text-align: center;
}

#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}
</style>
