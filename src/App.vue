<template>
 <div>
  <StudentVue  :userName="student.name" :point="student.score"/>
  <StudentForm @updateData="updateStudent"/>
</div>
</template>

<script>
import StudentVue from './components/Student.vue';
import StudentForm from './components/StudentForm.vue';


export default {
  name: 'App',
  emits:['updateData'],
  components: {
    StudentVue,
    StudentForm
    
  },
  data(){
    return{
      student:{
        name:'Zeynep Mirzooğlu',
        score:80,
      }
    }
  },
  methods:{
    updateStudent(nameStudent,scoreStudent){
      this.student ={
        name:nameStudent,
        score:scoreStudent,
      }
    }
  }
}
</script>

<style>

</style>
