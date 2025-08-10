<template>
<SeccionHeader />
<SeccionOpenData />
<SeccionFooter />
<!--<CustomCursor :config='{ highlighted_tags: [ "a", "button", ".text-res-1", ".circ-met", ".text-effect", ".menu-item" ], 
                            transform_time: ".2s", click_effect_enabled: false }' />-->
<WhatsAppWidget phone="542494279833" :quick_replies="quick_replies" />
</template>

<script setup>
import { ref } from 'vue'

const quick_replies = ref([
  {
    text: "Desarrollo de APP's",
    phone: "542494279833"
  },
  {
    text: "Testing",
    phone: "542494067516"
  },
])

import SeccionFooter from './components/SeccionFooter.vue'
import SeccionHeader from './components/SeccionHeader.vue';
import SeccionOpenData from './components/SeccionOpenData.vue';
</script>

