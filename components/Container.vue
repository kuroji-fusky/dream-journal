<script lang="ts" setup>
const props = defineProps<{
	t?: string
	d?: string
}>()

useHead({
	title: props.t,
	meta: [
		{ name: "description", content: props.d },
		{ property: "og:title", content: props.t },
		{ property: "og:description", content: props.d },
		{ property: "og:type", content: "website" },
		{ name: "twitter:card", content: "summary" },
		{ name: "twitter:title", content: props.t },
		{ name: "twitter:description", content: props.d },
	]
})
</script>

<template>
	<main data-app-content-wrap="false">
		<slot />
	</main>
</template>