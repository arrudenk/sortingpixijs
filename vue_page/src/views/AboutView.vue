<script setup lang="ts">
import WelcomeItem from '../components/WelcomeItem.vue'
import DyvoIcon from '../components/icons/IconDyvo.vue'
import EcosystemIcon from '../components/icons/IconEcosystem.vue'
import IconEvolution from "@/components/icons/IconEvolution.vue";
import IconNetEnt from "@/components/icons/IconNetEnt.vue";
</script>

<template>
  <div class="about">
    <p> My programming journey</p>
    <WelcomeItem>
      <template #icon>
        <DyvoIcon />
      </template>
      <template #heading>Work in <a href="www.linkedin.com/company/dyvo-gaming" target="_blank" rel="noopener">Dyvo Gaming</a></template>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <IconEvolution/>
      </template>
      <template #heading>Work in <a href="https://www.linkedin.com/company/evolution-global" target="_blank" rel="noopener">Evolution Gaming</a></template>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <IconNetEnt/>
      </template>
      <template #heading>Work in <a href="https://www.netent.com/en/" target="_blank" rel="noopener">NetEnt</a></template>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <EcosystemIcon/>
      </template>
      <template #heading>Education</template>
    </WelcomeItem>
  </div>
</template>