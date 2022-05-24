<template>
	<div>
		<div class="row">
			<div class="col-md-12" style="text-align:center;">
				<ul>
					<li>this is first contents</li>
				</ul>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name:"componentBlog",
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
