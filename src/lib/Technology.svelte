<script>
  const iconGroups = [
    [
      null,
      {src: 'javascript'},
      {src: 'python'},
      {src: 'nodejs'},
      {src: 'java'},
      null
    ],

    [
      {src: 'golang'},
      {src: 'reactjs'},
      {src: 'angular'},
      {src: 'graphql'},
      {src: 'nestjs'},
      {src: 'springio'}
    ],
    
    [
      {src: 'amazon_aws'},
      {src: 'microsoft_azure'},
      {src: 'google_cloud'},
      {src: 'kubernetes'},
      {src: 'docker'},
      {src: 'terraformio'}
    ],
    [
      null,
      {src: 'apache_kafka'},
      {src: 'rabbitmq'},
      {src: 'elastic'},
      {src: 'elasticco_kibana'},
      null
    ]
  ];

  const cdnUrl = 'https://www.vectorlogo.zone/logos'
</script>

<section
  id="technology"
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
                  src={`${cdnUrl}/${icon.src}/${icon.src}-icon.svg`}
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
