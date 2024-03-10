<template>
    <main>      
      <div class="containerBlue text-center bg-primary d-flex align-items-center" >
        <div class="row">
          <div class="col-5 ">
            <input class="form-control " type="text" name="buscarCargo" id="" placeholder=" Busca por cargo, salario, ubicación o empresa">
          </div>
  
          <div class="col-7 d-flex align-items-center dropdown ">
            <button class="btn btn-primary btn-search dropdown-toggle botones" type="button" data-bs-toggle="dropdown" aria-expanded="false">Área</button>
            <button class="btn btn-primary btn-search dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">Cargo</button>
            <button class="btn btn-primary btn-search dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">Salario</button>
            <button class="btn btn-primary btn-search dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">Ubicación</button>
          </div>    
        </div>
      </div>  
    </main>
  </template>  

<script>
  export default{
  name:"BlueComp"  
}
</script>

<style scoped>
.containerBlue{
  height: 70px;
}

.btn-search{
  border-radius: 40px;
  border: solid 1px white;
  color: white;
  font-size: 13px;
}

.btn-search:hover{
  background-color: white !important;
  color: black !important;
}
</style>