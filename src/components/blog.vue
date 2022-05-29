<template>
	<div>
		<div class="row justify-content-center align-items-center" style="min-height:100px;">
			<div class="col-md-12 text-center">blog</div>
		</div>
		<div class="row justify-content-center" style="margin-bottom:10px;">
			<div class="col-md-4">
				<div class="card" style="width: 300px; margin:auto">
					<div style="position:absolute; width:100%; top:-20px;">
						<span>2022-05-27 23:20</span>
					</div>
					<img src="https://images.velog.io/images/jojo_devstory/post/dae32386-bffc-40c3-b866-5c1e64516902/Android%2010_0.jpg" class="card-img-top" alt="...">
					<div class="card-body">
						<h5 class="card-title" style="font-size:20px;">안드로이드 공부의 시작</h5>
						<p class="card-text" style="white-space: nowrap; overflow: hidden; text-overflow: ellipsis;">사실 시작은 4월에 전주에서부터 시작했지만, 제대로 강의를 수강한 것은 이직하고 부터다</p>
						<div class="row">
							<div class="col-md-12">
								<a href="#" class="btn btn-primary" style="width:100%;" @click="prepare()">Go somewhere</a>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name:"componentBlog",
	methods: {
		prepare: function() {
			alert("준비중입니다.");
		}
	}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
