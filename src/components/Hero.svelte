<script>
  export let width = "960";
  export let height = "400";
  export let image;
  if (!image) {
    image = `https://picsum.photos/${width}/${height}`;
  }
</script>

<style>
  img {
    width: 100%;
    height: auto;
    min-height: 400px;
  }
</style>

<img src={image} alt="Hero" />
<!-- <img src="black-and-white.jpg" alt="Hero" /> -->
