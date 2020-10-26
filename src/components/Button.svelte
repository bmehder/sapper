<script>
  export let text = "Learn More";
  export let link = "/contact";
</script>

<style>
  a {
    display: inline-block;
    width: 200px;
    background: #f06;
    color: white;
    margin: 1em 0 1em;
    padding: 1em 1.5em;
    text-decoration: none;
    font-weight: bold;
    text-align: center;
    border-radius: 5px;
    transition: 0.2s ease-in-out;
  }
  a:hover {
    transform: scale(0.99);
    transition: 0.2s ease-in-out;
  }
</style>

<a href={link}>{text}</a>
