<script lang="ts">
  import type { HeroProfileButton } from "./types";

  export let data: HeroProfileButton
</script>

<a
  title={data.label}
  aria-label={data.label}
  href={data.link}
  target="_blank"
  class="mx-2">
  <img alt={data.imgAlt} src={data.imgSrc} class="h-auto w-10 rounded-lg" />
</a>