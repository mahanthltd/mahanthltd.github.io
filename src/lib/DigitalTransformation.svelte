<script lang="ts">
  import DigitalTransformation from '../assets/digital_transformation.png';

  const digitalTransforms = [
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
</script>

<section id="digital-transformation">
  <div
    class="relative max-w-screen-xl p-4 px-4 py-16 mx-auto bg-white dark:bg-gray-800 sm:px-6 lg:px-8"
  >
    <div class="relative">
      <div
        class="lg:grid lg:grid-flow-row-dense lg:grid-cols-2 lg:gap-8 lg:items-center"
      >
        <div class="ml-auto lg:mr-6 lg:max-w-2xl">
          <p
            class="text-base font-semibold leading-6 text-sky-500 dark:text-sky-400 uppercase"
          >
            Digital Transformation
          </p>
          <h4
            class="mt-2 text-2xl font-extrabold leading-8 text-gray-900 dark:text-white sm:text-3xl sm:leading-9"
          >
            Our Strategy
          </h4>
          <p class="mt-4 text-lg leading-6 text-gray-600">
            Our digital transformation strategy helps organizations to define
            and articulate their digital goals to create broad organizational
            alignment.
          </p>
          <p class="mt-4 text-lg leading-6 text-gray-600">
            We help to assess the organization’s digital maturity and readiness
            for change to then pinpoint the required critical capabilities and
            competencies
          </p>
        </div>
        <div class="relative mt-10 space-y-6 relative-20 lg:mt-0">
          <img
            src={DigitalTransformation}
            rel="external"
            size="6"
            alt="DigitalTransformation"
          />
        </div>
      </div>
    </div>
  </div>

  <div
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
  </div>
</section>
