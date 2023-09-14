<script>
	export let slice;
</script>

<ul>
	<li><a aria-label="linkedin link" href="{slice.primary.linkedin.url}"><iconify-icon icon="mdi:linkedin"></iconify-icon></a></li>
	<li><a aria-label="instagram link" href="{slice.primary.twitter.url}"><iconify-icon icon="mdi:instagram"></iconify-icon></a></li>
	<li><a aria-label="twitter link" href="{slice.primary.instagram.url}"><iconify-icon icon="mdi:twitter"></iconify-icon></a></li>
</ul>

<style>
	iconify-icon {
    	color: white;
		font-size: 1.5em;
		margin-top: .5em;
		margin-right: 10px;
	}
	ul {
		width: 100%;
    	display: flex;
    	flex-direction: row;
    	justify-content: center;
    	align-items: center;
	}
	li {
		list-style-type: none;
	}
</style>