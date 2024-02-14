<script lang="ts">
  import ProfileLinkButton from './profileLinkButton.svelte';
  import profileData from '$lib/data/profileInfo.json'
</script>

<section id="contact" class="bg-white dark:bg-gray-900">
  <div class="mx-auto flex items-center gap-y-16 px-4 py-24 lg:mt-12 sm:py-32 lg:max-w-7xl lg:px-8">
    <div class="w-full mr-auto">
      <h1 class="max-w-5xl mb-4 text-2xl font-extrabold tracking-tight md:text-5xl dark:text-white">
        <span class="mb-5">📧 제가 마음에 드셨다면, 연락주세요! 😊</span>
      </h1>
      <hr />
      <ul class="flex flex-col my-6 font-light text-gray-500 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400">
        {#each profileData.links as profileLink}
          <ProfileLinkButton data={profileLink} />
        {/each}
      </ul>
    </div>
  </div>
</section>