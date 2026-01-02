<template>
  <NuxtLayout>
    <div id="app-wrapper">
      <NuxtPage />
    </div>
  </NuxtLayout>
</template>
<style>
@import "tailwindcss";
@import "@nuxt/ui";

  /* 폰트 설정 (실제 폰트 파일로 교체하세요) */
  @font-face {
      font-family: 'inadoong';
      src: url('https://blog.howeverina.studio/font/Griun_InaDoongdoong-Rg.woff2') format('woff2'); /* 실제 경로 입력 */
      font-weight: 700;
      font-style: normal;
  }
  @font-face {
    font-family: 'Pretendard';
    src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/pretendard@1.0/Pretendard-Regular.woff2') format('woff2');
    font-weight: 400;
    font-display: swap;
}

@font-face {
    font-family: 'Pretendard';
    src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/pretendard@1.0/Pretendard-Bold.woff2') format('woff2');
    font-weight: 700;
    font-display: swap;
}

  :root {
    --accent: #86D7FF;
    --line: #ddd;
    --bg: #f5f5f5;
    --accentbg: #c8edff;
    --fg: #1e1f25;
  }

  body {
    font-family: 'Pretendard';
    color: var(--fg);
    background-color: var(--bg);
    font-size: 18px;
    line-height: 1.8;
  }

  input {
    font-family: 'inadoong';
    color: var(--fg);
  }
        
</style>