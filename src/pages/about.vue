<template>
  <v-container class="py-8" max-width="1000">
    <h1 class="text-h4 font-weight-bold mb-4">About</h1>

    <v-row>
      <v-col cols="12" md="4">
        <v-avatar size="120" class="mb-4">
          <v-img src="/avatar.png" alt="Avatar" />
        </v-avatar>
        <div class="text-subtitle-1">しーある</div>
        <div class="text-body-2 text--secondary">VRChat World Programmer</div>
      </v-col>

      <v-col cols="12" md="8">
        <v-card rounded="lg" variant="tonal">
          <v-card-text class="pa-6" style="white-space: pre-line">
            <div class="mb-3">
              VRChat 向けのワールド制作とインタラクティブなゲームシステムの実装を中心に活動しています。UdonSharp と Unity を組み合わせたギミック設計やネットワーク挙動の調整を得意としています。
            </div>

            <div class="mb-2 font-weight-medium">主な担当</div>
            <ul style="margin-top:0; margin-bottom:12px; padding-left:20px">
              <li>UdonSharp によるゲームロジック開発</li>
              <li>ワールド内 UI / UX 設計</li>
              <li>パフォーマンス最適化とデバッグ</li>
            </ul>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>

    <v-row class="mt-6">
      <v-col cols="12">
        <v-card rounded="lg" variant="tonal">
          <v-card-text class="pa-6">
            <div class="font-weight-medium mb-2">使用言語・フレームワーク</div>

            <v-row>
              <v-col cols="12" md="4">
                <div class="mb-2 font-weight-medium">VRChat / Unity</div>
                <div class="d-flex flex-wrap">
                  <v-chip size="small" class="ma-1">UdonSharp</v-chip>
                  <v-chip size="small" class="ma-1">C#</v-chip>
                  <v-chip size="small" class="ma-1">VRChat SDK</v-chip>
                  <v-chip size="small" class="ma-1">Unity</v-chip>
                </div>
              </v-col>

              <v-col cols="12" md="4">
                <div class="mb-2 font-weight-medium">Web Development</div>
                <div class="d-flex flex-wrap">
                  <v-chip size="small" class="ma-1">Vue.js</v-chip>
                  <v-chip size="small" class="ma-1">Vuetify</v-chip>
                  <v-chip size="small" class="ma-1">Spring</v-chip>
                  <v-chip size="small" class="ma-1">JavaScript</v-chip>
                </div>
              </v-col>

              <v-col cols="12" md="4">
                <div class="mb-2 font-weight-medium">Programming Languages</div>
                <div class="d-flex flex-wrap">
                  <v-chip size="small" class="ma-1">Python</v-chip>
                  <v-chip size="small" class="ma-1">Java</v-chip>
                  <v-chip size="small" class="ma-1">JavaScript</v-chip>
                  <v-chip size="small" class="ma-1">C#</v-chip>
                </div>
              </v-col>
            </v-row>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
// 詳細な About ページ
</script>
