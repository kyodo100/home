<template>
  <div id="page-view">
    <!--
      URLが変わった場合、ここに表示されます. -->

    <!--
      属性順: v-if, v-for => v-on => v-bind => ref => id => class -->
    
    <router-view id="router-view"/>
  </div>
</template>

<style>
  /* 共通のCSS */

  * {
    /* paddingとborderを含めてwidthやheightを計算する */
    box-sizing: border-box;
    /* スクロール端のバインド効果をなくす */
    overscroll-behavior: none;
  }

  html {
    scrollbar-width: thin;
    scrollbar-color: rgba(0,0,0,0.7) transparent;
    /* 色の登録 */
    /* MenuElement */
    --leather-backgroud: rgb(134, 26, 24);
    --leather-backgroud-dark: rgb(106, 29, 28);
    --leather-backgroud-light: rgb(116, 24, 23);
    --menu-scroll-bar: rgba(94, 26, 25, 0.756);
    --leather-front: rgb(94, 26, 25);
    --leather-seam: rgb(88, 24, 23);
  }

  body {
    width: 100lvw;
    height: 100lvh;
    margin: 0px;
    padding: 0px;
    overflow-x: hidden;
  }

  .a {
    color: #000000;
    cursor: pointer;
    text-decoration: none;
    -webkit-text-size-adjust: 100%;
    tap-highlight-color: transparent;
    -webkit-tap-highlight-color: transparent;
  }

  .btn {
    text-decoration: none;
    -webkit-text-size-adjust: 100%;
    tap-highlight-color: transparent;
    -webkit-tap-highlight-color: transparent;
    appearance: none;
    font-style: normal;
    font-variant-ligatures: normal;
    font-variant-caps: normal;
    font-variant-numeric: normal;
    font-variant-east-asian: normal;
    font-variant-alternates: normal;
    font-variant-position: normal;
    font-weight: normal;
    font-stretch: condensed;
    font-size: 1rem;
    font-family: inherit;
    font-optical-sizing: none;
    font-kerning: normal;
    font-feature-settings: normal;
    font-variation-settings: inherit;
    text-rendering: auto;
    color: inherit;
    letter-spacing: normal;
    word-spacing: normal;
    line-height: inherit;
    text-transform: capitalize;
    text-indent: 0px;
    text-shadow: none;
    display: inline-block;
    text-align: center;
    cursor: pointer;
    background-color: transparent;
    margin: 0px;
    padding-block: 0px;
    padding-inline: 0px;
    border-width: 0px;
    border-style: none;
    border-color: transparent;
    border-image: initial;
  }

</style>

<script setup lang="ts">
import { createHead } from 'unhead';

createHead()
</script>