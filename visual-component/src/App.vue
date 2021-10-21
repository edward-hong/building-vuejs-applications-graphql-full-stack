<template>
  <div id="app">
    <MaterialCardBox
      header="Material Card Header"
      sub-header="Card Sub Header"
      show-media
      show-actions
      img-src="https://picsum.photos/300/200"
      :main-text="
        `
        The path of the righteous man is beset on all sides by the iniquities
        of the selfish and the tyranny of evil men.`
      "
    >
      <template v-slot:action>
        <MaterialButton backgroundColor="#027be3" textColor="#fff"
          >Action 1</MaterialButton
        ><MaterialButton backgroundColor="#26a69a" textColor="#fff" is-flat
          >Action 2</MaterialButton
        >
      </template>
    </MaterialCardBox>
  </div>
</template>

<script>
  import MaterialButton from './components/MaterialButton.vue'
  import MaterialCardBox from './components/MaterialCardBox'

  export default {
    name: 'app',
    components: {
      MaterialCardBox,
      MaterialButton,
    },
  }
</script>

<style>
  body {
    font-size: 14px;
  }
</style>
