<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****2211 完成了硕士论文 AIGC 版权归属开题报告撰写"
  },
  {
    "text": "用户 189****9900 获得了 5 章逻辑严密的毕业论文大纲"
  },
  {
    "text": "用户 131****4455 完成了结构方程模型 (SEM) 研究方法设计"
  },
  {
    "text": "用户 156****7788 生成了查重率从 25% 降至 8% 的学术润色段落"
  },
  {
    "text": "用户 173****3311 取得了学术论文技术路线图制作指南"
  }
]);
</script>
