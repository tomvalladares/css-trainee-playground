/**
 * Home
 */

<script>

export default {

	name: "Home",

	data: () => ({ text: "En un mundo imaginario arriba aparecerá un texto y abajo aparecerá otro" })
}
</script>

<template lang="pug">

.home.d-grid




	p.open-sans.text-center {{ text }}
	p.open-sans.text-center 01
	p.open-sans.text-center 02
	p.open-sans.text-center 03

	router-link(to="/section").button Go to Section

</template>

<style lang="stylus" scoped>
@require ('../stylus/color.styl')

.button
	background 	color-button
	color 		color-button-text
	text-align  center

.home
	grid-template-columns 	1fr 1fr 1fr
	grid-template-rows    	1fr 1fr 1fr
	height 					100vh
	padding 				50px

p
	color 		color-paragraph


</style>
