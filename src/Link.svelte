<script lang="ts">
  import css from "./styles/Link.module.css";

  export let url: string;
</script>

<a href={url}>
  <div class={`${css.link} ${css.otherDims}`}>
    <div class={css.label}>
      <slot />
    </div>
  </div>
</a>
