<script>
  export let props = [
    { name: "linkedin", url: "https://www.linkedin.com/in/jankostrzewa/" },
    { name: "github", url: "https://github.com/jankostrzewa" }
  ];
</script>

<style>
  footer {
    margin: 0;
    padding: 0;
    background-color: #ccc;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-end;
  }

  a{
    margin: 0 1em;
  }
</style>

<footer>
  Copyright © Jan Kostrzewa 2019
  {#each props as socialMedia}
    <div>
      <a href={socialMedia.url}>
        <i class="fab fa-{socialMedia.name}" />
      </a>
    </div>
  {/each}
</footer>
