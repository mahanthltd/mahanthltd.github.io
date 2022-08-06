<script lang="ts">
  import TailwindCss from './TailwindCSS.svelte';
  import Nav from './lib/Nav.svelte';
  import Hero from './lib/Hero.svelte';
  import Project from './lib/Project.svelte';
  import Services from './lib/services.svelte';
  import Footer from './lib/Footer.svelte';
  import Technology from './lib/Technology.svelte';
  import DigitalTransformation from './lib/DigitalTransformation.svelte';
</script>

<TailwindCss />
<main
  class="mb-20 space-y-20 overflow-hidden sm:mb-32 sm:space-y-32 md:mb-40 md:space-y-40"
>
  <Nav />
  <Hero />
  <Services />
  <DigitalTransformation />
  <Technology />
  <Project />
  <Footer />
</main>
