

<template>
   <!-- Передаем в календаль events- массив событий-->
  <Calendar :events="events"/>   <!-- Используем компонент "Календарь" -->
</template>



<script>
import Calendar from './components/Calendar.vue'    // Импортируем компонент "Календарь"

export default {
  name: 'App',
  components: {
   Calendar  // Описание используемых компонентов: "Календарь"
  },
  data(){
    return{
      events:[
       {id:1,name:"Презентация",date: new Date(2021, 18, 10, 16,30), type:"red"},
       {id:2,name:"Лабораторная",date: new Date(2021, 18, 10, 18,30), type:"green"},
       {id:3,name:"семинар",date: new Date(2021, 18, 10, 18,30), type:"orange"},
       {id:4,name:"Лабораторная",date: new Date(2021, 24, 10, 14), type:"green"},
       {id:5,name:"семинар",date: new Date(2021, 24, 10, 16), type:"orange"},
       {id:6,name:"Презентация",date: new Date(2021, 18, 10, 16,30), type:"red"},
       {id:7,name:"Лабораторная",date: new Date(2021, 18, 10, 18,30), type:"green"},
       {id:8,name:"семинар",date: new Date(2021, 18, 10, 18,30), type:"orange"},
       {id:9,name:"Лабораторная",date: new Date(2021, 24, 11, 14), type:"green"},
       {id:10,name:"семинар",date: new Date(2021, 24, 11, 16), type:"orange"}

      ]
    }
  }
}
</script>

