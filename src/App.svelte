<script>
  import { title, desc, socials, other } from "../vals.json";
  import Link from "./Link.svelte";
  import SocialLink from "./SocialLink.svelte";
</script>

<main>
  <h1>{title}</h1>
  <p>{desc}</p>

  <h2>Socials</h2>
  <div class="socialsGrid">
    {#each socials as item}
      <SocialLink
        alt={item[0]}
        url={item[1]}
        icon={`/${item[0].toLowerCase()}.svg`}
      />
    {/each}
  </div>

  <h2>Other links</h2>
  <div class="linksColumn">
    {#each other as link}
      <Link url={link[1]}>{link[0]}</Link>
    {/each}
  </div>

  <footer><span>Made with <span class="heart">♥</span> in Egham</span></footer>
</main>
