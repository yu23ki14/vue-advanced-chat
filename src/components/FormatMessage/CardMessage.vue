<template>
	<!-- eslint-disable-next-line vue/no-v-html -->
	<div class="vac-link-card-wrapper" v-html="content" />
</template>

<script>
export default {
	name: 'CardMessage',
	props: {
		content: { type: null, default: '' }
	}
}
</script>
