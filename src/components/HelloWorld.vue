<template>
<div>
  <form class="form-inline">
  
  <div class="form-group mx-sm-3 mb-2">
    <label for="inputPassword2" class="sr-only">Nombre</label>
    <input type="text" class="form-control" v-model="nombre" placeholder="Nombre">
  </div>
  
  <button type="button" @click="newUser(nombre)" class="btn btn-primary">Primary</button>
</form>
    
    

</div>

</template>

<script>
import calendar from '../assets/calendario.json'
export default {
  name: 'HelloWorld',
  data: function(){
    return{
       empresa: [],
       nombre:""
    };
    
  },
  methods:{
    newUser: function(n){
    
      this.empresa.push({Nombre:n, calendar})
      console.log(this.empresa)
    }
   
  }
 

}
</script>



