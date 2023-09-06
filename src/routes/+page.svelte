<script>
    import { SliceZone } from '@prismicio/svelte'
    import { components } from '$lib/slices' 
    
    export let data
</script>

<h1>{ data.title }</h1>
<p>{ data.content[0].text }</p>
<img src="{data.image.url}" alt="">

<!-- <pre>
    {JSON.stringify(data,null,2)}
</pre> -->

<SliceZone slices={data.slices} {components} />