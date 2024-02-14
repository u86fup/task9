<style lang="scss" scoped>
@import "~/assets/styles/task.scss";
@import "~/assets/styles/task_blue.scss";
</style>


<template>
	<div :class="color">

	<header>
		<h3>Chang Color</h3>
		<button class="black" @click="changeColor('color_black')"></button>
		<button class="blue" @click="changeColor('color_blue')"></button>
	</header>
	
	<section class="sidebar">
		<div class="burger"><img src="~/assets/img/icon_burger_w.svg" alt="burger"></div>
	</section>
	
	<section class="third">
		
		<i id="leftarrow" class="fas fa-chevron-left" style="color: white;"></i>
		
		<div class="search_bg">
			<p class="search">
			<img src="~/assets/img/icon_search.svg" alt="pic">
			</p>
		</div>
		
		<div class="type">
			<div id="yt" class="text">ALL</div>
			<div class="text">Type1</div>
			<div class="text">Type2</div>
			<div class="text">Type3</div>
			<div class="text">Type1</div>
			<div class="text">Type2</div>
			<div class="text">Type3</div>
		</div>
		
		<i id="rightarrow" class="fas fa-chevron-right" style="color: white;"></i>
	
	</section>
	
	
	
	<div class="list">
		<div class="x">
			<i class="fas fa-times" style="color: white;"></i>
		</div>
		
		<p><a href="#"><img src="~/assets/img/icon_home_w.svg" alt="pen">&nbsp; Home</a></p>
		<p><a href="#"><img src="~/assets/img/icon_info_w.svg" alt="pen">&nbsp; About</a></p>
		<p><a href="#"><img src="~/assets/img/icon_pen_w.svg" alt="pen">&nbsp; Post1</a></p>
		<p><a href="#"><img src="~/assets/img/icon_pen_w.svg" alt="pen">&nbsp; Post2</a></p>
		<p><a href="#"><img src="~/assets/img/icon_pen_w.svg" alt="pen">&nbsp; Post3</a></p>
	</div>

	<section class="abc">
		<div>
			<p>A</p>
			<p>C</p>
			<p>E</p>
			<p>G</p>
			<p>I</p>
		</div>
		
		<div>
			<p>B</p>
			<p>D</p>
			<p>F</p>
			<p>H</p>
			<p>J</p>
		</div>
	</section>
	
	<footer></footer>
		
	</div>
</template>

<script setup lang="ts">
const color = ref('color_black');
const changeColor = (value: string) => {
  color.value = value;
}
</script>


