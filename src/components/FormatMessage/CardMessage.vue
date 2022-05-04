<template>
	<a :href="href" class="vac-link-card-wrapper" target="_blank">
		<img :src="img" :alt="`${title}の画像`" class="vac-link-ogpimg" />
		<div class="vac-link-card-desc">
			<h3>{{ title }}</h3>
			<p>{{ href }}</p>
		</div>
		<svg-icon name="bookmark" />
	</a>
</template>

<script>
import SvgIcon from '../SvgIcon/SvgIcon'

export default {
	name: 'CardMessage',
	components: {
		SvgIcon
	},
	props: {
		title: { type: String, required: true },
		href: { type: String, required: true },
		img: { type: String, default: '' }
	}
}
</script>
