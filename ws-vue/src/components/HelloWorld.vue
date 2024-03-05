<template> 
  
    <div class="card-body p-2 p-md-3" style="background-color: rgb(175, 175, 207);"> 
      <div class="row align-items-center">
        <div class="justify-content-center align-items-center col-md-1 col-3">
          <img src="favicon.ico" alt="" width="70" height="70" class="rounded"><img>
        </div>
        <div class="col-md-11 col-9" v-for="trabajo in trabajos" :key="trabajo.id" >
          <div class="row align-items-center">
            <div class="mb-2 col" >
              <a href="#" class="text-dark stretched-link d-inline d-md-inline-flex">
                <h2 class="bold pl-md-2 pr-md-2 mb-0 pb-0">{{ trabajos.titleVacante}}</h2>
                <section class="pl-md-2 d-md-inline-flex align-items-center text-wrap" >
                  <div class="text-truncated border dark text-dark text-capitalize" style="font-size: 0.8em; margin-bottom: 0px !important;">
                    <span></span>
                  </div>
                  <div class="text-truncated border dark text-dark text-capitalize" style="font-size: 0.8em; margin-bottom: 0px !important;">
                    <span></span>
                  </div>
                  <div class="text-truncated border dark text-dark text-capitalize" style="font-size: 0.8em; margin-bottom: 0px !important;">
                    <span></span>
                  </div>
                </section>
              </a>
            </div>
          </div>
          <div class="row pl-md-2 mt-1 flex-column flex-md-row" style="font-size: 0.9em;">
            <div class="text-truncated text-capitalize col"></div>            
            <div class="text-truncated text-capitalize col"></div>            
            <div class="text-truncated text-capitalize col"></div>            
            <div class="text-truncated text-capitalize col"></div>            
            <div class="text-truncated text-capitalize col"></div>            
          </div> 
        </div>   
      </div>            
    </div>
    
      

</template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }, 
  data(){
    return {
      trabajos: {
        id: 1,
        titleVacante: 'Analista de infraestructura',
        epresa: 'Expert Tech',
        skill: ['HTML', 'CSS','JS'],
        ciudad: "Medellín",
        salario: "1.9M - 2.1M COP",
        vacante: "Vacantes 1",
        about: "14 hours ago",
        publicacion: "publicacion numero 1"
      }
    }
  },
    methods: {  
      publicacionMostrar() {
        
        const contenidoDiv = document.getElementById('hello');        

        contenidoDiv.innerHTML = `<div>
          <div class="card-body p-2 p-md-3" style="background-color: rgb(175, 175, 207);"> 
           <div class="row align-items-center">
             <div class="justify-content-center align-items-center col-md-1 col-3">
               <img src="favicon.ico" alt="" width="70" height="70" class="rounded"><img>
             </div>
             <div class="col-md-11 col-9" v-for="(trabajo, indice) in trabajos" :key="indice">
                {{ trabajo }}
               <div class="row align-items-center">
                 <div class="mb-2 col" >
                   <a href="#" class="text-dark stretched-link d-inline d-md-inline-flex">
                     <h2 class="bold pl-md-2 pr-md-2 mb-0 pb-0"></h2>
                     <section class="pl-md-2 d-md-inline-flex align-items-center text-wrap" >
                       <div class="text-truncated border dark text-dark text-capitalize" style="font-size: 0.8em; margin-bottom: 0px !important;">
                         <span></span>
                       </div>
                       <div class="text-truncated border dark text-dark text-capitalize" style="font-size: 0.8em; margin-bottom: 0px !important;">
                         <span></span>
                       </div>
                       <div class="text-truncated border dark text-dark text-capitalize" style="font-size: 0.8em; margin-bottom: 0px !important;">
                         <span></span>
                       </div>
                     </section>
                   </a>
                 </div>
               </div>
               <div class="row pl-md-2 mt-1 flex-column flex-md-row" style="font-size: 0.9em;">
                 <div class="text-truncated text-capitalize col"></div>            
                 <div class="text-truncated text-capitalize col"></div>            
                 <div class="text-truncated text-capitalize col"></div>            
                 <div class="text-truncated text-capitalize col"></div>            
                 <div class="text-truncated text-capitalize col"></div>            
               </div> 
             </div>   
           </div>        
         </div>
       </div>      
       }`

      
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
</style>

    
