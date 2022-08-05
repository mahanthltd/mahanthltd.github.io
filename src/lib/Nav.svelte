<script>
  let menus = [
    {id: 'Team', name: '/team'},
    {id: 'Projects', name: '/projects'},
    {id: 'Blog', name: '/reports'}
  ];
</script>

<div
  class="relative flex items-center justify-between pt-6 text-sm font-semibold leading-6 lg:pt-8 text-slate-700 dark:text-slate-200"
>
  <svg viewBox="0 0 248 31" class="w-auto h-5 text-slate-900 dark:text-white" />
  <div class="flex items-center">
    <div class="items-center hidden md:flex">
      <nav>
        <ul class="flex items-center space-x-8">
          {#each menus as menu}
            <li>
              <a
                class="hover:text-sky-500 dark:hover:text-sky-400"
                href={menu.name}>{menu.id}</a
              >
            </li>
          {/each}
        </ul>
      </nav>
    </div>
  </div>
</div>
