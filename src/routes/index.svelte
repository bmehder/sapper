<script>
  import Hero from "../components/Hero.svelte";
  import Button from "../components/Button.svelte";
</script>

<style>

</style>

<svelte:head>
  <title>Home</title>
</svelte:head>

<Hero width="960" height="400" image="" />

<section>
  <h1>My Website</h1>

  <h3>Lore Impsum</h3>
  <p>
    Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolores rerum modi
    asperiores at a cupiditate nam nisi, veniam architecto officiis pariatur
    suscipit commodi quos harum incidunt quasi reiciendis. Deserunt natus eos
    commodi recusandae fuga odio dolorem facilis? Temporibus qui incidunt
    tempore consectetur mollitia facere minus corporis modi ipsa! Molestias
    accusamus aut accusantium?
  </p>

  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates
    exercitationem quo earum magnam facere iure repellat incidunt odio harum
    possimus.
    <a href="/">Excepturi liquid</a>
    unde explicabo omnis ad facere tempora sed, molestias recusandae dolore
    labore corrupti id deserunt! Praesentium quasi asperiores quibusdam ea atque
    perspiciatis corrupti consectetur, voluptatem ex, accusamus amet maxime
    maiores vitae porro similique voluptatum sequi molestiae doloribus? Quam
    nesciunt maxime repellat ratione eos nobis non esse, vel reiciendis libero
    iusto. Delectus, quas accusantium.
  </p>

  <div class="flex dark">
    <ul>
      <li>Lorem ipsum, dolor sit amet consectetur adipisicing.</li>
      <li>Lorem ipsum dolor sit amet.</li>
      <li>Lorem ipsum dolor sit amet consectetur.</li>
    </ul>

    <Button text="Send Us A Message" />
  </div>

</section>
