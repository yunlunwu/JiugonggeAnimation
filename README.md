# 基礎需求
請在 手機版面 390 * 844px (Chrome: iphone 12 Pro 模擬器) 大小之下，依照指定提供的資料內容，製作一個有可收合側邊選單的展示頁面，包含三個部分:

## 主頁面-側邊選單收合按鈕
請製作一個按鈕，無指定樣式，可開啟/收合側邊選單即可
## 主頁面-九宮格動畫
請切出一個九宮格，部分格子會不停閃爍。並且在指定的格子內(四個角落)有一顆球，球會向右移動一段距離

九宮格需要垂直置中於下方區塊 (示意圖中灰色底色區塊)

每個格子的規格如下 (寬度為螢幕寬均分, 間隔距離自行決定即可)

    height: 100px;
    border: black solid 2px;
    background: radial-gradient(circle, rgba(113,81,95,1) 81%, rgba(0,0,0,1) 100%);

    指定格子(右上, 正中, 右下) 會不停閃爍 (需有漸變or淡入淡出效果)
    透明度 100% -> 60% -> 100% -> 60% ...

    指定的球 (四個角落)
    width: 30px;
    height: 30px;
    background-color: #A5F12B;

### 球往右方移動時會在所有九宮格的上方，不被任一九宮格蓋住，且全程保持透明度 100% 請務必使球不會閃爍 (因動畫透明度影響 or 其他原因導致)
## 側邊選單
請依照上方給定的資料，產出側邊選單

主頁面的按鈕可以開啟側邊選單，點擊空白處可以關閉選單
側邊選單內每個項目都可以點擊，點擊後 highlight 選取中的項目，若該項目有子元素，會展開該層。
一次只會有一個展開且 highlight 的項目。

# Vue 3 + Vite

This template should help get you started developing with Vue 3 in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

## Install and use 
- Installation dependencies

```bash
cd JiugonggeAnimation

npm install

```

- run

```bash
npm run dev
```

- build

```bash
npm run build
```