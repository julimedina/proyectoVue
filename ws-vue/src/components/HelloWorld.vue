
<template> 

  
    <div class="card-body p-2 p-md-3" > 
      <div class="row align-items-center componentes card-body"  v-for="(trabajo, index) in trabajos" :key="index" >
        <div class="justify-content-center align-items-center col-md-1 col-3">
          <img src="favicon.ico" alt="" width="70" height="70" class="rounded">
        </div>
        <div class="container">
          <div class="col-md-11 col-9 ">
          <div class="row align-items-center">
            <div class="mb-2 col" >
              <a href="#" class="text-dark stretched-link d-inline d-md-inline-flex" style="text-decoration: none;">
                <h2 class="bold pl-md-2 pr-md-2 mb-0 pb-0">{{ trabajo.titleVacante }}</h2>
                <section class="pl-md-2 d-md-inline-flex align-items-center text-wrap">
                  <div  class="text-truncated border dark text-dark text-capitalize">
                  </div>
                  <div class="text-truncated border dark text-dark text-capitalize" style="font-size: 0.8em; margin-bottom: 0px !important;">
                    <span>{{trabajo.titleVacante}}</span>
                  </div>
                  <div class="text-truncated border dark text-dark text-capitalize" style="font-size: 0.8em; margin-bottom: 0px !important;">
                    <span>{{trabajo.titleVacante}}</span>
                  </div>
                </section>
              </a>
            </div>
          </div>
          <div class="row pl-md-2 mt-1 flex-column flex-md-row" style="font-size: 0.9em;">
            <div class="text-truncated text-capitalize col"><span class="material-icons-outlined">
                                apartment
                                </span>{{trabajo.empresa}}</div>            
            <div class="text-truncated text-capitalize col"><span class="material-icons-outlined">
                                location_on
                            </span>{{trabajo.ciudad}}</div>            
            <div class="text-truncated text-capitalize col"><span class="material-icons-outlined">
                                payments
                            </span>{{trabajo.salario}}</div>            
            <div class="text-truncated text-capitalize col"><span class="material-icons-outlined">
                                supervisor_account
                                </span>{{trabajo.vacante}}</div>            
            <div class="text-truncated text-capitalize col"><span class="material-icons-outlined">
                                calendar_month
                                </span>{{trabajo.about}}</div>            
          </div> 
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
      trabajos: [{
        id: 1,
        titleVacante: 'Analista de infraestructura',
        empresa: 'Expert Tech',
        skills: ['HTML', 'CSS','JS'],
        ciudad: "Medellín",
        salario: "1.9M - 2.1M COP",
        vacante: "Vacantes 1",
        about: "24 hours ago",
        publicacion: "publicacion numero 0"
      },
      {
        id: 2,
        titleVacante: 'Analista de infraestructura',
        empresa: 'Expert Tech',
        skills: ['HTML', 'CSS','JS'],
        ciudad: "Medellín",
        salario: "1.9M - 2.1M COP",
        vacante: "Vacantes 1",
        about: "15 hours ago",
        publicacion: "publicacion numero 1"
      },
      {
        id: 3,
        titleVacante: 'Analista de infraestructura',
        empresa: 'Expert Tech',
        skills: ['HTML', 'CSS','JS'],
        ciudad: "Medellín",
        salario: "1.9M - 2.1M COP",
        vacante: "Vacantes 1",
        about: "14 hours ago",
        publicacion: "publicacion numero 2"
      }
    ]
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
.componentes{
    border: solid 1px lightgray;
    margin-top: 20px;
    border-radius: 5px;
    
}

.componentes:hover{
    -webkit-box-shadow: 11px 24px 24px 5px rgba(0,0,0,0.75);
    -moz-box-shadow: 11px 24px 24px 5px rgba(0,0,0,0.75);
    box-shadow: 11px 2px 24px 5px lightgray;
}

.buton-requisitos{
    border: solid 1px black;
    font-size: 12px;
    width: 14%;
    border-radius: 45px;
    padding-left: 0;
    padding-right: 0;
   
}

</style>

 