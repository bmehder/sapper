<script>
  import Footer from "../components/Footer.svelte";
  export let segment;
</script>

<style>
  main {
    position: relative;
    min-height: 65vh;
    max-width: 960px;
    margin: 0 auto 4em;
    background: white;
    /* box-shadow: 0 1em 2em rgba(0, 0, 0, 0.2); */
    /* box-shadow: 0 2em 4em rgba(0, 0, 0, 1),
      inset -4em -4em 2em rgba(255, 255, 255, 0.5); */
    box-shadow: 4em 4em 10em rgba(0, 0, 0, 0.4),
      0em -4em 8em rgba(255, 255, 255, 0.32);
    /* border-bottom-left-radius: 5px;
    border-bottom-right-radius: 5px; */
    border-radius: 5px;
  }
  ul {
    display: flex;
  }
  @media (max-width: 400px) {
    header div,
    header nav,
    ul {
      display: block;
      width: 100%;
    }
  }
  li {
    list-style-type: none;
  }
  a {
    text-decoration: none;
    text-transform: capitalize;
    padding: 1em;
    display: block;
    font-family: "Luckiest Guy", sans-serif;
    color: white;
    letter-spacing: 2px;
    /* text-shadow: 2px 3px 20px rgba(0, 0, 0, 1); */
    opacity: 0.5;
    transition: 0.2s ease-in-out;
  }
  a:hover,
  a.active {
    opacity: 1;
    transition: 0.2s ease-in-out;
  }
  header {
    max-width: 960px;
    margin: auto;
    display: flex;
    justify-content: center;
    align-items: center;
    background: #444;
  }
  div {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 960px;
    margin: 0 auto 0 0;
  }
  img {
    width: 200px;
    margin-left: -2em;
  }
  a {
    padding-bottom: 0;
  }
</style>

<header>
  <div>
    <a href="/">
      <img src="logo-2.svg" alt="Logo" />
    </a>
  </div>
  <nav>
    <ul>
      <li>
        <a class={segment === undefined ? 'active' : ''} href=".">home</a>
      </li>
      <li>
        <a class:active={segment === 'about'} href="about">about</a>
      </li>

      <!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
		     the blog data when we hover over the link or tap it on a touchscreen -->
      <li>
        <a rel="prefetch" class:active={segment === 'blog'} href="blog">blog</a>
      </li>
      <li>
        <a class:active={segment === 'components'} href="components">
          components
        </a>
      </li>
      <li>
        <a class:active={segment === 'contact'} href="contact">contact</a>
      </li>
    </ul>
  </nav>
</header>

<main>
  <slot />
</main>

<Footer legal="Copyright ©2020 Brad Mehder. All Rights reserved." />
