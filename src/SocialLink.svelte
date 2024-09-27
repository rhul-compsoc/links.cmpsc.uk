<script lang="ts">
  import css from "./styles/Link.module.css";

  export let url: string;
  export let icon: string;
  export let alt: string;
</script>

<a href={url}>
  <div class={`${css.link} ${css.socialDims}`}>
    <div class={css.label}>
      <object type="image/svg+xml" data={icon} aria-label={alt} class={css.svg}
        >{alt}</object
      >
    </div>
  </div>
</a>
