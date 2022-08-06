<script>
  let digitalTransforms = [
    {
      title: 'Innovation',
      description:
        'We are able to guide customers on their path to technology modernization and digital transformation.'
    },
    {
      title: 'Collaboration',
      description:
        'Ensuring you have a connected environment empowers employees, optimizes productivity and processes, and enhances teamwork. To achieve that level of collaboration, we build, and businesses implement, solutions that enable the continuous loop.'
    },
    {
      title: 'Experience',
      description:
        'The question most companies face today – the factor driving a lot of digital transformation – is how do you thrive in such a fast-paced marketplace? It can’t be a process where we get an understanding of your market and tell you what to do; our guidance has to be actionable enterprise-wide.'
    },
    {
      title: 'Infrastructure Modernization',
      description:
        ' Infrastructure modernization allows you to take operational and administrative expenses and repackage those dollars into programs that drive innovation.'
    },
    {
      title: 'Operational Excellence',
      description:
        'Everyone uses operational reporting, sales forecasting, and the typical standard metrics when running a business. Creating excellence in those environments means finding solutions that have ecosystem connectivity to the cloud and to capabilities that help companies do advanced things.'
    },
    {
      title: 'Information and Insights',
      description:
        ' When creating an innovative environment doing automatic builds and deployments, all of the metrics from that project need to go into the knowledge repository. With a consolidated knowledge repository, all of the systems living in your business ecosystem can interact with and access each other’s data, automatically sharing valuable insights with very little additional technical work.'
    }
  ];

  const iconGroups = [
    [
      null,
      {src: 'javascript'},
      {src: 'python'},
      {src: 'node-dot-js'},
      {src: 'java'},
      null
    ],

    [
      {src: 'react'},
      {src: 'angularjs'},
      {src: 'svelte'},
      {src: 'next-dot-js'},
      {src: 'nestjs'},
      {src: 'spring'}
    ],
    [
      {src: 'amazonaws'},
      {src: 'azuredevops'},
      {src: 'googlecloud'},
      {src: 'kubernetes'},
      {src: 'docker'},
      {src: 'terraform'}
    ],
    [
      null,
      {src: 'apachekafka'},
      {src: 'rabbitmq'},
      {src: 'elastic'},
      {src: 'kibana'},
      null
    ]
  ];

  const cdnUrl = 'https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/';
</script>

<section
  class="grid sm:grid-cols-2 lg:grid-cols-3 space-y-3 lg:space-y-3 lg:space-x-3 rounded-lg"
>
  {#each digitalTransforms as { title, description }}
    <div
      class="relative z-10 -mx-4 bg-[radial-gradient(164.75%_40%_at_30%_0%,#87CEFA_0%,#FFFFFF_48.73%)] py-10 px-5 shadow-lg sm:mx-0 sm:rounded-3xl sm:px-10"
    >
      <div
        class="px-10 py-4 mt-4 md:py-10 border-b border-0 dark:border-solid-darkLighterBg md:border-r lg:border-b-0 lg:ml-4 lg:mt-0 last:border-none"
      >
        <h3 class="text-xl mb-2 font-semibold">{title}</h3>
        <p class="text-base">{description}</p>
      </div>
    </div>
  {/each}
</section>

<section
  class="dark:bg-solid-darkLighterBg bg-solid-lightgray py-16 grid grid-cols-1 lg:grid-cols-2 md:px-5 lg:px-16 defer rounded-br-6xl lg:bg-blocks-three bg-no-repeat bg-contain bg-right rtl:bg-left"
>
  <div
    class="px-10 py-4 2xl:bg-opacity-0 bg-opacity-80 rounded-lg xl:bg-opacity-0"
  >
    <p
      class="text-base font-semibold leading-6 text-sky-500 dark:text-sky-400 uppercase"
    >
      Technical Expertise
    </p>

    <p class="mt-4 text-lg leading-6 text-gray-600">
      When it comes to difficulties of software development, it’s important to
      understand that sometimes, without true expertise, it is impossible to
      properly assess the core of the problem.
    </p>
    <p class="mt-4 text-lg leading-6 text-gray-600">
      The superpowers of our technical expert has the abilities to deal with
      ambiguities, embrace possibilities and solve extremely complex issues.
    </p>
  </div>
  <div class="relative mt-10 space-y-6 relative-20 lg:mt-0">
    {#each iconGroups as iconGroup}
      <div class="grid grid-cols-6">
        {#each iconGroup as icon}
          {#if icon}
            <div
              class="flex items-center justify-center w-16 h-16 bg-gray-100 lg:w-20 lg:h-20 rounded-2xl"
            >
              <div class="w-12 h-12 lg:w-16 lg:h-16">
                <img
                  class="object-contain h-full"
                  src={cdnUrl + icon.src + '.svg'}
                  alt={icon.src}
                />
              </div>
            </div>
          {:else}
            <div>&nbsp;</div>
          {/if}
        {/each}
      </div>
    {/each}
  </div>
</section>
