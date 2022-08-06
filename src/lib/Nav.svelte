<script>
  let menus = [
    {id: 'Digital Transformation', name: '#digital-transformation'},
    {id: 'Services', name: '#services'},
    {id: 'Technology', name: '#technology'},
    {id: 'Projects', name: '#project'},
    {id: 'Blog', name: '#blog'},
    {id: 'Team', name: '#team'}
  ];
  function scrollIntoView({target}) {
    const el = document.querySelector(target.getAttribute('href'));
    if (!el) return;
    el.scrollIntoView({
      behavior: 'smooth'
    });
  }
</script>

<div
  class="relative flex items-center justify-between pt-6 text-sm font-semibold leading-6 lg:pt-8 text-slate-700 dark:text-slate-200"
>
  <svg viewBox="0 0 248 31" class="w-auto h-5 text-slate-900 dark:text-white" />
  <div class="flex items-center">
    <div class="items-center hidden md:flex">
      <nav>
        <ul class="flex items-center space-x-8">
          {#each menus as { name, id }}
            <li>
              <a
                class="hover:text-sky-500 dark:hover:text-sky-400"
                on:click|preventDefault={scrollIntoView}
                href={name}>{id}</a
              >
            </li>
          {/each}
        </ul>
      </nav>
    </div>
  </div>
</div>
