<script lang="ts">
	// `data` comes from +page.ts automatically
	export let data: {
		company: string;
		year: number;
	};
</script>

<h1>About Us</h1>
<p>{data.company} was founded in {data.year}.</p>