<template>
  <UApp>
    <div class="bg-dark-background">
      <ButtonComp :variant="'primary'" :is-bold="true">
        Try for Free
      </ButtonComp>

      <ButtonComp :variant="'primary'">
        Teste
      </ButtonComp>
    </div>
  </UApp>
</template>

<script setup>
import ButtonComp from './components/ButtonComp.vue';


</script>

