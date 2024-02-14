<script lang="ts">
  import ProjectItem from "./projectItem.svelte";
</script>

<section id="project" class="pt-12 bg-gray-50 dark:bg-gray-900">
  <div class="grid max-w-screen-xl px-4 py-4 mx-auto lg:pt-16 lg:pb-8">
    <div class="mr-auto place-self-center lg:col-span-7">
      <h2 class="max-w-5xl mb-4 text-4xl font-extrabold tracking-tight md:text-5xl xl:text-6xl dark:text-white">
        <span class="mb-3">🖼️ 프로젝트</span>
      </h2>
    </div>
  </div>
  <hr class="bg-black max-w-screen-xl mx-5 h-0.5" />
  <div class="block md:flex">
    <div class="flex-none text-lg text-gray-600 font-light md:flex-1">
      <ProjectItem />
    </div>
  </div>
  <div class="flex flex-col m-5 p-5">
    ※ 아래는 2020년 이전의 프로젝트를 모은 노션 페이지입니다. (클릭 시 노션 페이지로 이동)
    <a
      class="text-blue-500"
      href="https://tkddn204.notion.site/07ca748d29fa4ebbb2d6384cda31be13?v=a8753caeeef3406192abf82450732f35">
      2020년 이전 프로젝트
    </a>
  </div>
</section>