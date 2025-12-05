<script setup>
import EventCard from '@/components/EventCard.vue'
import { ref } from 'vue'

const events = ref([
  {
    id: 1,
    category: 'conference',
    title: 'Vue Conference',
    discription: 'A conference about all things Vue.js',
    location: 'New York City',
    date: '2024-09-15',
    time: '10:00 AM',
    petallowed: true,
    organization: 'Vue Community',
  },
  {
    id: 2,
    category: 'meetup',
    title: 'Vue.js Meetup',
    discription: 'A casual meetup for Vue.js enthusiasts',
    location: 'San Francisco',
    date: '2024-10-20',
    time: '6:00 PM',
    petallowed: false,
    organization: 'SF Vue Group',
  },
  {
    id: 3,
    category: 'workshop',
    title: 'Vue Workshop',
    discription: 'Hands-on workshop to learn Vue.js basics',
    location: 'Chicago',
    date: '2024-11-05',
    time: '9:00 AM',
    petallowed: true,
    organization: 'Tech Workshops Inc.',
  },
])
</script>

<template>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
