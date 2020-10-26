<script>
  import Video from "../../components/Video.svelte";
</script>

<svelte:head>
  <title>Components</title>
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css" />
  <style>
    .controls .fa-play {
      color: #28a745;
    }
    .controls .fa-stop {
      color: #dc3545;
    }
    .controls .fa-pause {
      color: #fff;
    }
  </style>
</svelte:head>

<section>
  <h1>Custom Video API</h1>
  <Video
    file="https://player.vimeo.com/external/354485035.sd.mp4?s=530fed84f1567d1a7784e877e98e053cff203686&profile_id=139&oauth2_token_id=57447761"
    poster="https://picsum.photos/800/450"
    loop />

  <Video />
</section>
