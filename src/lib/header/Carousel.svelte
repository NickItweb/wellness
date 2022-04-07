<script>
  import Carousel from 'svelte-carousel'

</script>
<Carousel
  autoplay
  autoplayDuration={5000}
  autoplayProgressVisible
  pauseOnFocus
>
  {#each colors as { color, text } (color)}
    <Color {color} {text} />
  {/each}
</Carousel>
