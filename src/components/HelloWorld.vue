<script setup lang="ts"></script>

<template>
  <div>12312</div>
  <h1>1</h1>
  <h1>2</h1>
  <h1>3</h1>
  <button @click="modal = true">Open Modal</button>
  <div class="ml-2 relative inline-block">
    <button @click.stop="dropdown = !dropdown">Toggle Dropdown</button>
    <div v-if="dropdown" v-on-click-outside.bubble="dropdownHandler" class="dropdown-inner">
      Click outside of the dropdown to close it.
    </div>
  </div>
  <div v-if="modal" ref="modalRef" class="modal">
    <div class="inner">
      <button class="button small" title="Close" @click="modal = false">𝖷</button>
      <p class="heading">Demo Modal</p>
      <p>Click outside of the modal to close it.</p>
    </div>
  </div>
</template>

<style scoped></style>
