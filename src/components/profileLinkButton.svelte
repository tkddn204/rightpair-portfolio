<script lang="ts">
  import type { HeroProfileButton } from "./types";
  import { dev } from '$app/environment';
  import { PUBLIC_BASE_URL } from '$env/static/public';

  export let data: HeroProfileButton
</script>

<li class="hover:bg-gray-100">
  <a
    title={data.label}
    aria-label={data.label}
    href={data.link}
    target="_blank"
    class="flex flex-row mx-2">
    <img alt={data.imgAlt} src={dev ? data.imgSrc : new URL(PUBLIC_BASE_URL, data.imgSrc).href } class="h-auto w-10 rounded-lg" />
    <span class="m-5">{data.label}</span>
  </a>
</li>