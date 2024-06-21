<template>   
    <div class="container" > 
      <div class="componentes card-body p-3" v-for="(trabajo, index) in trabajos" :key="index">
             
        <div class="col-md-11 col-9 ">
          
            <div class="row align-items-center">
              <div class="justify-content-center align-items-center col-md-1 col-3">
          <img :src="rutaImagen" alt="" width="70" height="70" class="rounded">
        </div> 
              <div class="mb-2 col" >
                <a href="#" class="text-dark stretched-link d-inline d-md-inline-flex" style="text-decoration: none;">
                  <strong><h4 class="bold pl-md-2 pr-md-2 mb-0 pb-0">{{ trabajo.titleVacante }}</h4></strong>
                  <section class="pl-md-2 d-md-inline-flex align-items-center text-wrap">                    
                    <div class="text-truncated border dark text-dark text-capitalize m-1" style="font-size: 0.8em; margin-bottom: 0px !important;" v-for="(skill, index) in trabajo.skills" :key="index">
                      <span> {{ skill }}</span>
                    </div>                    
                  </section>
                </a>
              </div>
            </div>
            <div class="row  mt-1 flex-column flex-md-row" style="font-size: 0.9em;">
              <div class="text-truncated text-capitalize col"><span class="material-symbols-outlined">apartment</span>{{trabajo.empresa}} </div>            
              <div class="text-truncated text-capitalize col"><span class="material-symbols-outlined">location_on</span>{{trabajo.ciudad}} </div>            
              <div class="text-truncated text-capitalize col"><span class="material-symbols-outlined">local_atm</span> {{trabajo.salario}}</div>            
              <div class="text-truncated text-capitalize col"><span class="material-symbols-outlined">group</span>{{trabajo.vacante}} </div>            
              <div class="text-truncated text-capitalize col"><span class="material-symbols-outlined">calendar_month</span>{{trabajo.about}} </div>            
              <div class="text-truncated text-capitalize col"><span class="material-symbols-outlined"></span></div>            
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
      trabajos:[{
        id: 1,
        titleVacante: 'Director Tecnico II',
        rutaImagen: '@/assets/metf.png',
        empresa: 'OFFIMEDICA SA',
        skills: ['tecnical Knoledge', 'Attitude To service','Liderazgo'],
        ciudad: "Bucaramanga",
        salario: "1.9MCOP",
        vacante: "Vacantes 1",
        about: "11 hours ago"        
      },
      {
        id: 2,
        titleVacante: 'Analista de infraestructura',
        rutaImagen: '@assets/metf.png',
        empresa: 'Expert Tech',
        skills: ['HTML', 'CSS','JS'],
        ciudad: "Medellín",
        salario: "1.9M - 2.1M COP",
        vacante: "Vacantes 1",
        about: "24 hours ago"        
      },
      {
        id: 3,
        titleVacante: 'Analista de operaciones',
        rutaImagen: '@/assets/metf.png',
        empresa: 'Intexus',
        skills: ['Sales', 'Client service','Attitude To service'],
        ciudad: "presencial(Bogotá)",
        salario: "1M - 1.4M COP",
        vacante: "Vacantes 1",
        about: "2 days ago"        
      },
      {
        id: 4,
        titleVacante: 'Ejecutivo Comercial',
        rutaImagen: require('@/assets/metf.png'),
        empresa: 'Metlife Medellin',
        skills: ['Comercial Aggressiveness', 'Negotiation capacity'],
        ciudad: "Medellín",
        salario: "2M - 6M COP",
        vacante: "Vacantes 3",
        about: "3 days ago"        
      },
      {
        id: 5,
        titleVacante: 'Senior QA automation',
        rutaImagen: require('@/assets/metf.png'),
        empresa: 'Think Us',
        skills: ['Jenkins', 'Postman','Cypress'],
        ciudad: "Remoto",
        salario: "2M - 2.5M COP",
        vacante: "Vacantes 3",
        about: "2 days ago"        
      }

    ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>



.componentes{    

    border: solid 1px rgb(189, 188, 188);
    border-radius: 5px; 
    margin: 1rem;  
  position: relative;
    
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

 