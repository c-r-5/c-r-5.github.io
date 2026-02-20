<template>
  <v-container class="py-8" max-width="1000">
    <h1 class="text-h4 font-weight-bold mb-4">Projects</h1>

    <v-row>
      <v-col
        v-for="project in projects"
        :key="project.title"
        cols="12"
        md="6"
      >
        <v-card
          :href="project.link"
          rounded="lg"
          target="_blank"
          variant="tonal"
        >
          <v-card-item>
            <template #prepend>
              <v-avatar color="primary" size="48">
                <v-icon>{{ project.icon }}</v-icon>
              </v-avatar>
            </template>
            <v-card-title class="text-wrap">{{ project.title }}</v-card-title>
            <v-card-subtitle>{{ project.subtitle }}</v-card-subtitle>
          </v-card-item>
          <v-card-text>
            <p class="mb-3" style="white-space: pre-line">{{ project.description }}</p>
            <v-chip-group>
              <v-chip
                v-for="tech in project.technologies"
                :key="tech"
                size="small"
                variant="outlined"
              >
                {{ tech }}
              </v-chip>
            </v-chip-group>
          </v-card-text>
          <v-card-actions>
            <v-spacer />
            <v-icon>mdi-open-in-new</v-icon>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
const projects = [
  {
    title: 'スコフィごいた Scofi-Goita',
    subtitle: 'VRChat World',
    description: `VRChat 向けのボードゲームギミックを実装。
Udon を使用してゲームロジックと UI 制御を開発しました。`,
    icon: 'mdi-checkerboard',
    link: 'https://vrchat.com/home/world/wrld_5d74d392-d90b-4b24-8da7-cdedca7965a0',
    technologies: ['UdonSharp', 'C#', 'Unity'],
  },
  {
    title: 'めたモグ - Metamogphose Lab.',
    subtitle: 'VRChat World',
    description: `Virtual Sanrio Puroland 内の育成ゲームのプログラマーとして参加。
Udon によるゲームシステムの実装を担当しました。`,
    icon: 'mdi-sprout',
    link: 'https://vrchat.com/home/world/wrld_cb8a80b2-de72-49d2-ac5d-d750f948877e',
    technologies: ['UdonSharp', 'C#', 'Unity'],
  },
]
</script>
