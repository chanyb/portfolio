<template>
	<div>
		<div class="row justify-content-center align-items-center" style="min-height:100px;">
			<div class="col-md-12 text-center">blog</div>
		</div>
		<div class="row justify-content-center" style="margin-bottom:10px;">
			<div class="col-md-4">
				<div class="card" style="width: 300px; margin: auto;">
					<div style="position:absolute; width:100%; top:-20px;">
						<span>2022-05-27 23:20</span>
					</div>
					<img src="https://images.velog.io/images/jojo_devstory/post/dae32386-bffc-40c3-b866-5c1e64516902/Android%2010_0.jpg" class="card-img-top" alt="...">
					<div class="card-body">
						<h5 class="card-title" style="font-size:20px;">안드로이드 공부의 시작</h5>
						<p class="card-text" style="white-space: nowrap; overflow: hidden; text-overflow: ellipsis;">사실 시작은 4월에 전주에서부터 시작했지만, 제대로 강의를 수강한 것은 이직하고 부터다</p>
						<div class="row">
							<div class="col-md-12">
								<button href="" class="btn btn-primary" style="width:100%;" @click="prepare()">바로가기</button>
							</div>
						</div>
					</div>
				</div>
			</div>
			<div class="col-md-4">
				<div class="card" style="width: 300px; margin:auto">
					<div style="position:absolute; width:100%; top:-20px;">
						<span>2022-05-30 13:29</span>
					</div>
					<img src="https://images.velog.io/images/jojo_devstory/post/dae32386-bffc-40c3-b866-5c1e64516902/Android%2010_0.jpg" class="card-img-top" alt="...">
					<div class="card-body">
						<h5 class="card-title" style="font-size:20px;">안드로이드 생명주기</h5>
						<p class="card-text" style="white-space: nowrap; overflow: hidden; text-overflow: ellipsis;">안드로이드 생명주기는 Activity의 생명주기와 Fragment 생명주기, Service 생명주기 등 다양하게 존재한다. 현재 내가 또다른 어떤 생명주기를 모르고 있는지를 모른다.. </p>
						<div class="row">
							<div class="col-md-12">
								<button href="" class="btn btn-primary" style="width:100%;" @click="prepare()">바로가기</button>
							</div>
						</div>
					</div>
				</div>
			</div>
			<div class="col-md-4">
				<div class="card" style="width: 300px; margin:auto">
					<div style="position:absolute; width:100%; top:-20px;">
						<span>2022-06-01 09:01</span>
					</div>
					<img src="https://images.velog.io/images/jojo_devstory/post/dae32386-bffc-40c3-b866-5c1e64516902/Android%2010_0.jpg" class="card-img-top" alt="...">
					<div class="card-body">
						<h5 class="card-title" style="font-size:20px;">Activity & Fragment</h5>
						<p class="card-text" style="white-space: nowrap; overflow: hidden; text-overflow: ellipsis;">화면을 구성하는 방법에는 Activity와 Fragment를 사용할 수 있다. Activity는 UI를 구성하는 가장 기본적인 요소인데 사용자의 입장에서 보면 그냥 한 화면에 불과하지만, 개발자의 입장에서 보면 Activity는 2가지로 구분이 된다. 1) View: 있는 그대로의 화면을 구성하는 View 2)ViewModel 혹은 Controller: View와 Model을 연결하는 ViewModel이기도하며, 의존성이 높아지면 점점 Controller에 가까워진다. 안드로이드에서는 어떻게 구현하느냐에 따라 MVC, MVP, MVVM의 디자인 패턴을 가질 수 있다. 이처럼 Activity만을 사용해도 상관없지만, Fragment가 등장함에 따라 SPA(Single-Page-Application)의 개발이 가능하게 되었다. Fragment는 단독으로 사용할 수 없으며 반드시 Activity내부에서 사용해야 한다. 최근에는 SPA를 위하여 1개의 Activity위에 다수의 Fragment로 구현하는 것이 트렌드인 것 같다.(약간의조사를 통한 뇌피셜) 하지만, 대부분의 자료들이 Activity를 기반으로 설명 하고있기 때문에, 실제로 적용하는 것은 안드로이드에 대한 고수준의 지식을 요구하는 것 같다..!</p>
				
						<div class="row">
							<div class="col-md-12">
								<button href="" class="btn btn-primary" style="width:100%;" @click="prepare()">바로가기</button>
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
