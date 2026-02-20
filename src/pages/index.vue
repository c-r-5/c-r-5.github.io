<template>
  <v-container class="py-12" max-width="1000">
    <div class="text-center mb-8">
      <v-avatar size="120" class="mb-4">
        <v-img alt="Avatar" src="/avatar.png" />
      </v-avatar>
      <h1 class="text-h4 font-weight-bold mb-2">しーある</h1>
      <p class="text-subtitle-1 mb-4">VRChat World Programmer / UdonSharp</p>
      <div class="d-flex justify-center ga-3">
        <v-btn to="/about" variant="outlined">About</v-btn>
        <v-btn to="/projects" variant="outlined">Projects</v-btn>
        <v-btn to="/contact" variant="outlined">Contact</v-btn>
      </div>
    </div>

    <v-card rounded="lg" variant="tonal">
      <v-card-text>
        <div class="text-h6 mb-2">ようこそ — しーあるのポートフォリオへ</div>
        <div class="mb-4">UdonSharp を用いた VRChat ワールド、ゲームロジック構築を中心に活動しています。制作物やスキルは各ページでご覧いただけます。</div>
      </v-card-text>
    </v-card>
  </v-container>
</template>

<script setup>
// simple landing page
</script>
