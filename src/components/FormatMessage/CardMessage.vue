<template>
	<a :href="href" class="vac-link-card-wrapper" target="_blank">
		<img :src="img" :alt="`${title}の画像`" />
		<div class="vac-link-card-desc">
			<h3>{{ title }}</h3>
			<p>{{ href }}</p>
		</div>
	</a>
</template>

<script>
export default {
	name: 'CardMessage',
	props: {
		title: { type: String, required: true },
		href: { type: String, required: true },
		img: { type: String, default: '' }
	}
}
</script>
