<template>
	<div>
		<div class="row">
			<div class="col-md-12">
				<h1>{{ msg }}</h1>
			</div>
		</div>
		<div class="row">
			<div id="skillBody" class="col-md-12">
				<div>
					<h3>Language</h3>
				</div>
				<div class="row">
					<span class="item" @click="toggleItem('javascript')">Javascript</span>
					<span class="item" @click="toggleItem('python')">Python</span>
					<span class="item" @click="toggleItem('jsp')">JSP</span>
					<span class="item" @click="toggleItem('html')">HTML</span>
					<span class="item" @click="toggleItem('css')">CSS</span>
					<span class="item" @click="toggleItem('java')">Java</span>
					<span class="item" @click="toggleItem('c')">C, C++</span>
				</div>
				<div class="row">
					<h3>Frameworks</h3>
				</div>
				<div class="row">
					<span class="item" @click="toggleItem('vue')">Vue.js</span>
					<span class="item" @click="toggleItem('nativescript')">Nativescript</span>
					<span class="item" @click="toggleItem('bootstrap')">Bootstrap</span>
				</div>
				<div class="row">
					<h3>Software</h3>
				</div>
				<div class="row">
					<span class="item" @click="toggleItem('node')">Node.js</span>
					<span class="item" @click="toggleItem('dbeaver')">DBeaver</span>
					<span class="item" @click="toggleItem('git')">Git</span>
					<span class="item" @click="toggleItem('jira')">Jira</span>
				</div>
				<div class="row">
					<h3>Service</h3>
				</div>
				<div class="row">
					<span class="item preparing">Progress - Kendo UI for vue</span>
					<span class="item preparing">Progress - Kinvey</span>
				</div>
			</div>
			<div v-if="flag.itemToggle" class="col-md-6 window-mr">
				<div class="row" id="javascript" v-if="flag.itemToggle === 'javascript'">
					<div class="col-md-12">
						<img src="@/assets/metory_1.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>블록체인 기반 임상연구 플랫폼</p>
						<ul style="text-align: left">
							<li>frontend, backend 작성에 javascript를 기반으로하는 프레임워크인 vue.js, node.js를 활용했습니다.</li>
							<li>비동기/동기 처리와 ES6문법(() => {}, ${}, [...arr, obj] 등..)에 대한 이해가 있습니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="python" v-if="flag.itemToggle === 'python'">
					<div class="col-md-12">
						<img src="@/assets/python_1.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>오토인코더를 통한 iris data manifold 확인</p>
						<ul style="text-align: left">
							<li>tensorflow를 활용해 신경망 모델을 설계할 수 있습니다.</li>
							<li>파이썬의 문법을 이해하고 있으며, Selenium을 이용해 동적 크롤링을 하는 등의 작업이 가능합니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="jsp" v-if="flag.itemToggle === 'jsp'">
					<div class="col-md-12">
						<img src="@/assets/jsp_1.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>블록체인 기반 임상연구 플랫폼 - JSP</p>
						<ul style="text-align: left">
							<li>JSP를 사용해 세션에 값을 저장하고 유저의 인증 등의 Backend 개발을 할 수 있습니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="html" v-if="flag.itemToggle === 'html'">
					<div class="col-md-12">
						<img src="@/assets/html.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>HTML</p>
						<ul style="text-align: left">
							<li>HTML tag를 사용해 웹을 디자인 할 수 있으며, 코드를 확인하는 등의 작업을 통해 구조를 파악 할 수 있습니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="css" v-if="flag.itemToggle === 'css'">
					<div class="col-md-12">
						<img src="@/assets/css.png" style="max-height: 600px; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>CSS</p>
						<ul style="text-align: left">
							<li>css를 이용해 class, id, element 등 선택자들을 원하는 대로 꾸밀 수 있습니다.</li>
							<li>media query를 사용하여 반응형 웹을 만들 수 있습니다.</li>
							<li>keyframe을 사용하여 애니메이션을 적용시킬 수 있습니다.</li>
							<li>Boostrap, ant-design-of-vue 등 사용 경험을 바탕으로 타 css프레임워크(또는 모듈) 사용에도 빠르게 적응할 수 있습니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="java" v-if="flag.itemToggle === 'java'">
					<div class="col-md-12">
						<img src="@/assets/java_address_book.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>Java 개인 프로젝트 - 주소록</p>
						<ul style="text-align: left">
							<li>절차지향 언어와는 다른 객체지향 언어의 대표격인 java의 문법을 이해하고 개발 할 수 있습니다.</li>
							<li>JAR 파일을 만들어 jsp에서 사용 할 수 있습니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="c" v-if="flag.itemToggle === 'c'">
					<div class="col-md-12">
						<img src="@/assets/c.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>C, C++ - 수업 조교 경험 보유</p>
						<ul style="text-align: left">
							<li>메모리 관리에 대해 이해하고 개발 할 수 있습니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="git" v-if="flag.itemToggle === 'git'">
					<div class="col-md-12">
						<img src="@/assets/git_1.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>https://github.com/chanyb</p>
						<ul style="text-align: left">
							<li>git을 이용한 버전 관리, 협업이 가능합니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="vue" v-if="flag.itemToggle === 'vue'">
					<div class="col-md-12">
						<img src="@/assets/vue_blur.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>대상자관리 시스템</p>
						<ul style="text-align: left">
							<li>vuex를 이용한 상태관리를 할 수 있으며 axios를 이용한 request를 통해 개발 할 수 있습니다.</li>
							<li>proxy table을 이용해 CORS 환경에서 개발 한 경험이 있습니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="nativescript" v-if="flag.itemToggle === 'nativescript'">
					<div class="col-md-12">
						<img src="@/assets/nativescript.jpg" style="max-height: 700px; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>전자동의 앱 ARBO</p>
						<ul style="text-align: left">
							<li>하이브리드 앱 프레임워크 중 하나인 nativescript를 사용하여 안드로이드, ios에서 모두 작동하는 앱을 개발 할 수 있습니다.</li>
							<li>알람, local-notification, 진동, 위치감지, 동작감지, 생체인증 등의 native 기능들을 적용할 수 있습니다.</li>
							<li>firebase를 이용한 push notification을 사용 할 수 있습니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="dbeaver" v-if="flag.itemToggle === 'dbeaver'">
					<div class="col-md-12">
						<img src="@/assets/dbeaver.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>dbeaver를 활용한 데이터베이스 관리</p>
						<ul style="text-align: left">
							<li>데이터베이스 관리 도구인 dbeaver에서 SQL을 통해 DB를 분석하거나 데이터의 CRUD를 진행할 수 있습니다.</li>
							<li>기존에 사용되던 DB를 분석하고 migration한 경험이 있습니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="jira" v-if="flag.itemToggle === 'jira'">
					<div class="col-md-12">
						<img src="@/assets/jira.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>jira를 활용한 애자일 방식 프로젝트 진행</p>
						<ul style="text-align: left">
							<li>새로운 프로젝트의 시작에 jira를 활용하여 화면 별 이슈를 나눈 뒤 개발을 진행하였고 '개발↔피드백' 과정을 유연하게 진행한 경험이 있습니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="node" v-if="flag.itemToggle === 'node'">
					<div class="col-md-12">
						<img src="@/assets/nodejs.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>nodejs, postman을 활용한 API 개발 및 테스트</p>
						<ul style="text-align: left">
							<li>nodejs의 express 프레임워크를 사용해 RESTful API를 개발할 수 있습니다.</li>
						</ul>
					</div>
				</div>
				<div class="row" id="bootstrap" v-if="flag.itemToggle === 'bootstrap'">
					<div class="col-md-12">
						<img src="@/assets/bootstrap.png" style="width: 80%; border: 1px solid black" />
					</div>
					<div class="col-md-12">
						<!-- description -->
						<p>bootstrap 프레임워크를 사용한 UI 개발</p>
						<ul style="text-align: left">
							<li>bootstrap의 Grid system, css, component를 이용한 반응형 프론트엔드 디자인이 가능합니다.</li>
						</ul>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "HelloWorld",
	props: {
		msg: String,
	},
	methods: {
		moveLeft: function () {
			var mainFrame = document.getElementById("main");
			mainFrame.classList.add("moveLeft");
		},
		toggleItem: function (val) {
			var skillBody = document.getElementById("skillBody");

			var targetClass = skillBody.classList;

			if (targetClass.length === 1) {
				skillBody.classList.add("col-md-6");
				skillBody.classList.add("moveLeft");
				skillBody.classList.remove("col-md-12");

				skillBody.addEventListener(
					"animationend",
					() => {
						this.flag.itemToggle = val;
					},
					false,
				);
			} else {
				this.flag.itemToggle = val;
			}
		},
	},
	data() {
		return {
			flag: {
				itemToggle: false,
			},
		};
	},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.item {
	margin-right: 10px;
}
.item:hover {
	color: #238038;
	cursor: pointer;
}
.preparing {
	color: gray;
}
.preparing:hover {
	color: gray;
	cursor: default;
}

@-webkit-keyframes moveLeft {
	from {
		left: 30vh;
	}
	to {
		left: 0px;
	}
}

.moveLeft {
	animation-name: moveLeft;
	animation-duration: 1s;
	animation-fill-mode: forwards;
}

@media all and (min-width: 1200px) {
	.window-mr {
		padding-right: 10%;
	}
}
</style>
