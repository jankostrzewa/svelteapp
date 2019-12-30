<script>
  export let url = "foo";
  export let label = "bar";
</script>

<style>
  .a {
    height: 100%;
    width: 100%;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: end;
    align-items: center;
  }

  .b {
    width: 80%;
    height: 3em;
    line-height: 3em;
    background-color: #ddd;
    text-transform: capitalize;
    margin-bottom: 1em;
    border-radius: 0.5em;
    cursor: pointer;
  }
</style>

<div class="a">
  <div class="b" onclick="window.location.href='{url}'">
    {label}
  </div>
</div>
<!-- on:click={(window.location = url)}-->
