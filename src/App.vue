

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
    // год-месяц (0-11)-день-час
    return{
      events:[
       {id:1,name:"Презентация",date: new Date(2021, 10, 18, 16,30), type:"red"},
       {id:2,name:"Лабораторная",date: new Date(2021, 10, 18, 18,30), type:"green"},
       {id:3,name:"семинар",date: new Date(2021, 10, 18, 18,30), type:"orange"},
       {id:4,name:"Лабораторная",date: new Date(2021, 10, 24, 14), type:"green"},
       {id:5,name:"семинар",date: new Date(2021, 11, 24, 16), type:"orange"},
       {id:6,name:"Презентация",date: new Date(2021, 10, 18, 16,30), type:"red"},
       {id:7,name:"Лабораторная",date: new Date(2021, 10, 18, 18,30), type:"green"},
       {id:8,name:"семинар",date: new Date(2021, 11, 10, 18,30), type:"orange"},
       {id:9,name:"Лабораторная",date: new Date(2021, 10, 22, 14), type:"green"},
       {id:10,name:"семинар",date: new Date(2021, 10, 24, 16), type:"orange"}

      ]
    }
  }
}
</script>

