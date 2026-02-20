<template>
  <v-footer app class="text-center">
    <div class="py-3 w-100">
      <a
        v-for="item in socials"
        :key="item.title"
        class="mx-2"
        :href="item.href"
        rel="noopener noreferrer"
        target="_blank"
        :title="item.title"
      >
        <v-btn
          :icon="item.icon"
          size="small"
          variant="text"
        />
      </a>
    </div>
  </v-footer>
</template>

<script setup>
  const socials = [
    {
      title: 'GitHub',
      icon: 'mdi-github',
      href: 'https://github.com/c-r-5',
    },
    {
      title: 'Twitter',
      icon: 'mdi-twitter',
      href: 'https://x.com/cs_c_r_5',
    },
    {
      title: 'VRChat',
      icon: 'mdi-virtual-reality',
      href: 'https://vrchat.com/home/user/usr_e3966a0b-b96e-46a1-854f-dd1b2b8ac544',
    },
  ]
</script>
