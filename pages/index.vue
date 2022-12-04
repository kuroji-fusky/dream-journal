<script lang="ts" setup>
const t = "Kuroji's Dream Journal"
const d = "A place to dump my weird ass dreams"
</script>

<template>
	<Container :t="t" :d="d">
		<header>
			<h1 class="heading">Kuroji's <span class="gradient-text">Dream Journal</span></h1>
			<p>{{ d }}</p>
		</header>
	</Container>
</template>

<style lang="scss" scoped>
.heading {
	@apply font-bold text-2xl xl:text-3xl;
}

.gradient-text {
	@apply bg-clip-text text-transparent bg-gradient-to-br from-red-400 to-blue-400;
}
</style>