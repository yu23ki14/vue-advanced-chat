<template>
	<div class="vac-link-card-wrapper">
		<img :src="img" :alt="`${title}の画像`" />
		{{ title }} {{ href }}
	</div>
</template>

<script>
export default {
	name: 'LinkCard',
	props: {
		title: { type: String, required: true },
		href: { type: String, required: true },
		img: { type: String, default: '' }
	}
}
</script>
