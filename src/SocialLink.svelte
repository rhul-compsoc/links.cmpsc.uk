<script lang="ts">
  import css from "./styles/Link.module.css";

  export let url: string;
  export let icon: string;
  export let alt: string;
</script>

<a href={url}>
  <div class={`${css.link} ${css.socialDims}`}>
    <div class={css.label}>
      <img src={icon} {alt} class={css.svg} />
    </div>
  </div>
</a>
