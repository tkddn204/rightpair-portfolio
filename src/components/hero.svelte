<script lang="ts">
  import ProfileLinkButton from './profileLinkButton.svelte';
  import profileData from '$lib/data/profileInfo.json'
</script>

<section id="hero" class="bg-emerald-50 dark:bg-gray-900">
  <div class="mx-auto grid grid-flow-row md:grid-flow-col items-center gap-y-16 px-4 py-24 lg:mt-12 sm:py-32 lg:max-w-7xl lg:px-8">

    <div class="m-3 lg:mt-0 lg:col-span-3 lg:flex">
      <img src="https://www.notion.so/image/https%3A%2F%2Fprod-files-secure.s3.us-west-2.amazonaws.com%2F6fff5f0a-b9dd-4c74-8f5d-f76aabefe27e%2Ff2ea367e-516a-4907-b92a-5c6a6da0a5cb%2Fphoto_2020-09-03_00-17-53.jpg?table=block&id=06de89e4-fd6c-471f-bf7b-01943c90fbbd&spaceId=6fff5f0a-b9dd-4c74-8f5d-f76aabefe27e&width=250&userId=590c4dcc-2370-4f43-b1ae-eb4e4f98da83&cache=v2" alt="mockup">
    </div>
    <div class="w-full mr-auto place-self-center lg:col-span-7">
      <h1 class="max-w-5xl mb-4 text-4xl font-extrabold tracking-tight md:text-5xl xl:text-6xl dark:text-white">
        <span class="mb-5">👋 안녕하세요!</span>
      </h1>
      <p class="text-2xl mb-10 leading-loose">
        주니어 <span class="text-4xl font-bold underline decoration-sky-500">웹 백엔드</span> 개발자,
        <br class="sm:hidden">
        <span class="text-5xl font-bold bg-yellow-200">한상우</span>입니다.
      </p>
      <hr class="bg-black mx-auto h-0.5" />
      <p class="flex flex-row my-6 font-light text-gray-500 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400">
        {#each profileData.links as profileLink}
          <ProfileLinkButton data={profileLink} />
        {/each}
      </p>
    </div>
  </div>
</section>