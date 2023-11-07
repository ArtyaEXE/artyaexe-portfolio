<script>
  import Header from "./components/common/Header.svelte";
  import About from "./components/About.svelte";
  import Projects from "./components/Projects.svelte";
  import Connection from "./components/Connection.svelte";
</script>

<div class="wrapper">
  <Header />
  <main>
    <About />
    <Projects />
    <Connection />
  </main>
</div>

<style>
  .wrapper {
    position: relative;
  }
</style>
