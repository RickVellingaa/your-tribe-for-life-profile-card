<script>
	export let data;
    console.log();
</script>

<pre>
    {JSON.stringify(data,null,2)}
</pre>

<h1>{data.page.data.title[0].text}</h1>
<p>{data.page.data.slices[0].primary.over[0].text}</p>