<template>
  <div class="events">
    <Exercise v-for="event in events" :src="event.image" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import Exercise from '@/components/Exercise.vue'

export default {
  name: 'Home',
  components: {
    Exercise
  },
  data() {
    return {
      events: [
        {
          id: 5928101,
          category: 'Chest',
          title: 'Bench Press',
          Equipment: 'Flat Bench, Barbell',
          image: '../assets/bench.jpg'
        },
        
      ]
    }
  }
}
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>



{
          id: 5928101,
          category: 'Chest',
          title: 'Bench Press',
          Equipment: 'Flat Bench, Barbell',
          image: '../assets/bench.jpg'
        },
//         {
//           id: 4582797,
//           category: 'Lower Back',
//           title: 'Deadlift',
//           Equipment: 'Barbell',
//           image: '../assets/deadlift.jpg'
//         },
//         {
//           id: 8419988,
//           category: 'Upper Back',
//           title: 'Lat Pulldown',
//           Equipment: 'Pully Tower',
//           image: '../assets/latpull.jpg'
//         },
//         {
//           id: 8419989,
//           category: 'Shoulder',
//           title: 'Shoulder Press',
//           Equipment: 'Dumbbells',
//           image: '../assets/shoulderpress.jpg'
//         },
//         {
//           id: 8419990,
//           category: 'Legs',
//           title: 'Squat',
//           Equipment: 'Barbell',
//           image: '../assets/squat.jpg'
//         },