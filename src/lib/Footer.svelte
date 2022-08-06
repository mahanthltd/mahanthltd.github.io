<script lang="ts">
  const siteMetadata = {
    author: 'Mahanth Limited'
  };
  import MailEncoded from '../assets/social-icons/mail.svg';
  import GitHubEncoded from '../assets/social-icons/github.svg';
  import LinkedInEncoded from '../assets/social-icons/linkedin.svg';
  import TwitterEncoded from '../assets/social-icons/twitter.svg';

  const digitalIcons = [
    {src: MailEncoded, href: 'mailto:durairaj@mahanthltd.co.uk', alt: 'email'},
    {src: GitHubEncoded, href: 'https://github.com/durairaj', alt: 'github'},
    {
      src: LinkedInEncoded,
      href: 'https://www.linkedin.com/company/mahanthlimited',
      alt: 'linkedin'
    },
    {
      src: TwitterEncoded,
      href: 'https://twitter.com/MahanthLimited',
      alt: 'twitter'
    }
  ];
</script>

<footer>
  <div class="flex flex-col items-center mt-16">
    <div class="flex mb-3 space-x-4">
      {#each digitalIcons as { src, href, alt }}
        <a target="_blank" class="h-4 cursor-pointer hover:scale-150 " {href}>
          <img
            {src}
            rel="external"
            class="h-4 cursor-pointer hover:scale-150 "
            {alt}
            size="6"
          /></a
        >
      {/each}
    </div>
    <div class="flex mb-2 space-x-2 text-sm text-gray-500 dark:text-gray-400">
      <div>{siteMetadata.author}</div>
      <div>{`© ${new Date().getFullYear()}`}</div>
    </div>
  </div>
</footer>
