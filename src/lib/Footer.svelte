<script lang="ts">
  const siteMetadata = {
    author: 'Mahanth Limited',
    name: 'durairaj'
  };
  import MailEncoded from '../assets/social-icons/mail.svg';
  import GitHubEncoded from '../assets/social-icons/github.svg';
  import LinkedInEncoded from '../assets/social-icons/linkedin.svg';
  import TwitterEncoded from '../assets/social-icons/twitter.svg';

  const emailTo = () => {
    const subject = 'Enquiry from Website';
    window.open(
      'mailto:' +
        siteMetadata.name +
        '@' +
        window.location.host +
        '?subject=' +
        subject,
      '_self'
    );
  };

  const gotoLink = (link) => {
    const newWindow = window.open(link);
    newWindow.opener = null;
  };
  const digitalIcons = [
    {src: MailEncoded, alt: 'email', onClick: emailTo},
    {
      src: GitHubEncoded,
      href: 'https://github.com/durairaj',
      alt: 'github',
      onClick: gotoLink
    },
    {
      src: LinkedInEncoded,
      href: 'https://www.linkedin.com/company/mahanthlimited',
      alt: 'linkedin',
      onClick: gotoLink
    },
    {
      src: TwitterEncoded,
      href: 'https://twitter.com/MahanthLimited',
      onClick: gotoLink,
      alt: 'twitter'
    }
  ];
</script>

<footer>
  <div class="flex flex-col items-center mt-16">
    <div class="flex mb-3 space-x-4">
      {#each digitalIcons as { src, href, alt, onClick }}
        <img
          {src}
          rel="external"
          class="h-4 cursor-pointer hover:scale-150 "
          on:click={() => onClick(href)}
          {alt}
          size="6"
        />
      {/each}
    </div>
    <div class="flex mb-2 space-x-2 text-sm text-gray-500 dark:text-gray-400">
      <div>{siteMetadata.author}</div>
      <div>{`© ${new Date().getFullYear()}`}</div>
    </div>
  </div>
</footer>
