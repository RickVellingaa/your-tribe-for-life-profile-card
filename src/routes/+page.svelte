<script>
    import { SliceZone } from '@prismicio/svelte'
    import { components } from '$lib/slices' 

    export let data
</script>



<!-- <article onl class="front">
    <div class="text-header">
        <h1>{ data.title }</h1>
        <h2>{ data.beroep[0].text }</h2>
    </div>
</article>

<article  class="back">
    <div class="text-header">
        <h1>{ data.title }</h1>
        <h2>{ data.beroep[0].text }</h2>
    </div>
    <div class="content">
        
    </div>
</article> -->


    <div class="content">
      <div class="front">
        <article>
            <div class="text-header">
                <h1>{ data.title }</h1>
                <h2>{ data.beroep[0].text }</h2>
                <img class="my-image" src="{ data.image.url }" alt="Foto van Rick Vellinga">
                <div class="socials">
                    <SliceZone slices={data.slices} {components} />
                </div>
            </div>
            <div class="text-content">
        
            </div>
            
        </article>
      </div>
      <div class="back">
        <article>
            <div class="text-header">
                <h1>{ data.title }</h1>
                <h2>{ data.beroep[0].text }</h2>
                <img src="{ data.image.url }" alt="Foto van Rick Vellinga">
                <div class="socials">
                    <SliceZone slices={data.slices} {components} />
                </div>
            </div>
            <div class="text-content">
                <h3>Over mij</h3>
                <p>{ data.content[0].text }</p>
            </div>
        </article>
      </div>
    </div>



