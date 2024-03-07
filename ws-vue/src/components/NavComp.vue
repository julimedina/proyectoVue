<template>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#"><img src="/public/img/logo-blue.png" alt=""></a>
    
    <div class="collapse navbar-collapse d-flex justify-content-end" id="navbarSupportedContent">
      <ul class="navbar-nav  mb-2 mb-lg-0">
        <li class="nav-item">
          <a href="" class="nav-link active" aria-current="page" >Empleos</a>
        </li>
        <li class="nav-item">
          <a href="" class="nav-link" >Bootcamp</a>
        </li>
        <li class="nav-item">
          <a href="" class="nav-link" >Sobre nosotros</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Para profesionales
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" >Inicio</a></li>
            <li><a class="dropdown-item" >Empleos</a></li>
            <li><a class="dropdown-item" >Cursos y retos</a></li>
            <li><a class="dropdown-item" >Preguntas</a></li>
            <li><a class="dropdown-item" >Profesores</a></li>
            <li><a class="dropdown-item" >Bootcamp</a></li>
          </ul>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Para empresas
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item">Inicio</a></li>
            <li><a  class="dropdown-item" >Publicar empleo</a></li>
            <li><a  class="dropdown-item" >Nuestro proceso</a></li>
            <li><a  class="dropdown-item" >Precios</a></li>
            <li><a  class="dropdown-item" >Pruebas online</a></li>
            <li><a toclass="dropdown-item" >Nómina</a></li>
            <li><a class="dropdown-item" >Blog</a></li>
            <li><a class="dropdown-item" >Comercial</a></li>
            <li><a  class="dropdown-item" >Calculadora de salario</a></li>
          </ul>
        </li>
       
      </ul>
    
    
            <button class="btn light button-espanol" type="submit"><span class="material-icons">
            language</span>Español
            </button>
            <button class="btn light button-espanol" type="submit"><span class="material-icons-outlined">
                notifications
            </span>
            </button>
            <button class="btn light button-espanol" >
                <span class="material-icons">
                account_circle
                </span>
            </button>
     
        
        
    </div>
  </div>
</nav>
    
</template>

<script>

export default{
  name:"NavComp",
 
}

</script>



<style>
.button-espanol{
    border: solid 1px lightgrey;
    font-size: 12px;
}
</style>