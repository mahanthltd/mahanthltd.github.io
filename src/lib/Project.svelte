
<script>

    const projects = [
          { company: 'To be updated', name: 'To be updated', technologyUsed: [], date:'To be updated',
        description: 'To be updated'},
        { company: 'To be updated', name: 'To be updated', technologyUsed: [], date:'To be updated',
        description: 'To be updated'},
  
      ];

    </script>
    
<div
  class="relative sm:pb-1 sm:ml-[calc(2rem+1px)] md:ml-[calc(3.5rem+1px)] lg:ml-[max(calc(14.5rem+1px),calc(30%-48rem))]"
>
  <div
    class="hidden absolute top-3 bottom-0 right-full mr-7 md:mr-[3.25rem] w-px bg-slate-200 dark:bg-slate-800 sm:block"
  />
  <div class="space-y-16">
    {#each projects as project}
    <article class="relative group">
      <div
        class="absolute -inset-y-2.5 -inset-x-4 md:-inset-y-4 md:-inset-x-6 sm:rounded-2xl group-hover:bg-slate-50/70 dark:group-hover:bg-slate-800/50"
      />
      <svg
        viewBox="0 0 9 9"
        class="hidden absolute right-full mr-6 top-2 text-slate-200 dark:text-slate-600 md:mr-12 w-[calc(0.5rem+1px)] h-[calc(0.5rem+1px)] overflow-visible sm:block"
        ><circle
          cx="4.5"
          cy="4.5"
          r="4.5"
          stroke="currentColor"
          class="fill-white dark:fill-slate-900"
          stroke-width="2"
        /></svg
      >
      <div class="relative">
        <h3
          class="pt-8 text-base font-semibold tracking-tight text-slate-900 dark:text-slate-200 lg:pt-0"
        >
          {project.name}
        </h3>
        <div
          class="mt-2 mb-4 prose prose-slate prose-a:relative prose-a:z-10 dark:prose-dark line-clamp-2"
        >
          <p>
         {project.description}
          </p>
        </div>
        <dl
          class="absolute left-0 top-0 lg:left-auto lg:right-full lg:mr-[calc(6.5rem+1px)]"
        >
          <dt class="sr-only">Date</dt>
          <dd class="text-sm leading-6 whitespace-nowrap dark:text-slate-400">
            <time datetime="2022-06-23T19:40:00.000Z">{project.date}</time>
          </dd>
        </dl>
      </div>
    </article>
    {/each}
  </div>
</div>
