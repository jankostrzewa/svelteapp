<script>
  import Header from "./Header.svelte";
  import Footer from "./Footer.svelte";

  export let name;

  let data = [{ url: 'http://www.jankostrzewa.com', label: 'Homepage' }, { url: '/contact', label: 'Contact' }, { url: '/var', label: 'Var' }];
</script>

<style>
  h1 {
    color: purple;
  }
</style>

<Header
  props={data} />
<h1>Hello {name}!</h1>
<Footer />
