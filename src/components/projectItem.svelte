<script lang="ts">
  import type { ProjectItem } from "./types";

  export let data: ProjectItem
</script>

<!--<a-->
<!--  title={data.title}-->
<!--  aria-label={data.title}-->
<!--  target="_blank"-->
<!--  class="mx-2">-->
<!--</a>-->
<div class="mb-6">
  <h3 class="font-semibold text-gray-900 pb-1 hover:underline hover:text-black">
  <a href={data.link}>{data.title}</a></h3>
  <p class="text-md text-gray-600 font-light">
    {data.content}
  </p>
</div>