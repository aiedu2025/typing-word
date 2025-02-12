<script setup lang="ts">
import Dialog from "@/components/dialog/Dialog.vue"
import BaseButton from "@/components/BaseButton.vue";
import {GITHUB} from "@/config/ENV.ts";

const emit = defineEmits([
  'close',
])

</script>

<template>
  <Dialog
      @close="emit('close')"
      title="反馈">
    <div class="feedback-modal">
      <div>
        给我发Email：<a href="mailto:aiedu2025@outlook.com">aiedu2025@outlook.com</a>
      </div>
      <p>平顶山舞钢智适应教育科技<hr></p>
        <span style="font-size: 15rem;color: gray;margin-bottom: 5rem;text-align: justify;text-align-last: justify;">
		大模型 + 自适应学习 = 专属Ai老师配置到家<br>
		不到300元/月 | 超传统1对1的效果 | 省钱有效
        </span>
		<div data-v-8eb5bd9e="" class="git-log"> 
		</div>
		<a :href="`https://v.douyin.com/iPDwV4nM`" target="_blank" style="font-size: 10rem;color: gray;margin-bottom: 5rem;">Build d2753d0 (dev) @2017-2025</a>
	  <!-- <img src="/vxmp封面S_250205Tel.png" alt="">  -->
      <div class="github">
		<!-- ai_edu2016
		在<a :href="GITHUB" target="_blank">Github</a>上给我提一个 
		<a :href="`${GITHUB}/issues`" target="_blank">Issue</a>
		2025Deepseek后ai时代<br>
		-->
		  
        <!-- 
        <div class="options">
          <BaseButton>
            <a :href="`${GITHUB}/`" title="10小时掌握完一学期知识点"
               target="_blank">中高考ai精准备考</a>
          </BaseButton>
          <BaseButton>
            <a :href="`${GITHUB}/`" title=""
               target="_blank">中学生ai全科辅导</a>
          </BaseButton>
          <BaseButton>
            <a :href="`${GITHUB}/`" title="松鼠ai 9折|赶考ai小状元 7折|内部会员 折上折"
               target="_blank">ai学习机内部团购</a>
          </BaseButton>
		  <BaseButton>
            <a :href="`${GITHUB}/grade/1`"
               target="_blank">小学</a>
          </BaseButton>
          <BaseButton>
            <a :href="`${GITHUB}/grade/7`"
               target="_blank">初中</a>
          </BaseButton>
          <BaseButton>
            <a :href="`${GITHUB}/grade/10`"
               target="_blank">高中</a>
          </BaseButton>
        </div>
		-->
      </div>
    </div>
  </Dialog>
</template>

<style scoped lang="scss">
@import "@/assets/css/variable";

.feedback-modal {
  width: 500rem;
  //height: 80vh;
  display: flex;
  flex-direction: column;
  background: var(--color-second-bg);
  align-items: center;
  padding: var(--space);
  //justify-content: center;
  color: var(--color-font-1);

  p {
    font-size: 30rem;
  }

  .github {
    display: flex;
    align-items: center;
    gap: var(--space);

    .options {
      display: flex;
      flex-direction: column;
      gap: 10rem;
    }
  }
}

</style>