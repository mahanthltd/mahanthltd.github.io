<script lang="ts">
  const siteMetadata = {
    email: 'durairaj@mahanthltd.co.uk',
    author: 'Mahanth Limited',
    github: 'https://github.com/durairaj',
    twitter: 'https://twitter.com/MahanthLimited',
    linkedin: 'https://www.linkedin.com/company/mahanthlimited'
  };
  import MailEncoded from '../assets/social-icons/mail.svg';
  import GitHubEncoded from '../assets/social-icons/github.svg';
  import LinkedInEncoded from '../assets/social-icons/linkedin.svg';
  import TwitterEncoded from '../assets/social-icons/twitter.svg';
</script>

<footer>
  <div class="flex flex-col items-center mt-16">
    <div class="flex mb-3 space-x-4">
      <img
        src={MailEncoded}
        rel="external"
        href={`mailto:${siteMetadata.email}`}
        class="h-4 cursor-pointer hover:scale-150 "
        alt="email"
        size="6"
      />
      <img
        src={GitHubEncoded}
        rel="external"
        href={siteMetadata.github}
        class="h-4 cursor-pointer hover:scale-150 "
        alt="github "
        size="6"
      />
      <img
        src={LinkedInEncoded}
        rel="external"
        href={siteMetadata.linkedin}
        class="h-4 cursor-pointer hover:scale-150"
        alt="github"
        size="6"
      />
      <img
        src={TwitterEncoded}
        rel="external"
        href={siteMetadata.twitter}
        class="h-4 cursor-pointer hover:scale-150 "
        alt="github"
        size="6"
      />
    </div>
    <div class="flex mb-2 space-x-2 text-sm text-gray-500 dark:text-gray-400">
      <div>{siteMetadata.author}</div>
      <div>{`© ${new Date().getFullYear()}`}</div>
    </div>
  </div>
</footer>
