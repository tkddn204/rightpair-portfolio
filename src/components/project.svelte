<script lang="ts">
  import ProjectItem from "./projectItem.svelte";
  import projectData from '$lib/data/projectData.json';
</script>

<section id="project" class="bg-white dark:bg-gray-900">
  <div class="grid max-w-screen-xl px-4 py-8 mx-auto lg:gap-8 xl:gap-0 lg:py-16 lg:grid-cols-12">
    <div class="mr-auto place-self-center lg:col-span-7">
      <h2 class="max-w-5xl mb-4 text-4xl font-extrabold tracking-tight md:text-5xl xl:text-6xl dark:text-white">
        <span class="mb-3">🖼️ 프로젝트</span>
      </h2>
    </div>
  </div>
  <hr/>
  <div class="block pt-12 md:flex">
    <div class="flex-none text-lg text-gray-600 font-light md:flex-1 md:pl-20 md:pr-20">
      {#each projectData as data}
        <ProjectItem data={data} />
      {/each}
    </div>
  </div>
</section>