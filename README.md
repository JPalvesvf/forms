# forms
<!DOCTYPE html>
<html lang="pt-br">
<head> 
  <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.11.2/css/all.css">

<script>
  
    function formatar(mascara, documento){
      var i = documento.value.length;
      var saida = mascara.substring(0,1);
      var texto = mascara.substring(i);
  
      if (texto.substring(0,1) != saida){
        documento.value += texto.substring(0,1);
        
        
      }
    }
</script>

</head>
<body>
  <div class="container">
      <nav class="navbar fixed-top navbar-expand-lg navbar-light bg-info">
        <a class="navbar-brand text-white" href="#">Home</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Alterna navegação">
      <span class="navbar-toggler-icon"></span>
    </button>
  
    <div class=" collapse navbar-collapse" id="navbarSite">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item active">
          <a class="nav-link text-white"  href="#"> Início <span class="sr-only">(Página atual)</span></a>
        </li>
        <li class="nav-item">
          <a class="nav-link text-white" href="#">Alunos</a>
        </li>
        <li class="nav-item ">
          <a class="nav-link text-white" href="#">Acesse o portal</a>
        </li>
  
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle text-white" href="#" id="navbarDropdownMenuLink" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
            Aulas
          </a>
          <div class="dropdown-menu" aria-labelledby="navbarDropdown">
            <a class="dropdown-item" href="#">Ciências</a>
            <a class="dropdown-item" href="#">história</a>
            <a class="dropdown-item" href="#">Geografia</a>
            <a class="dropdown-item" href="#">Matemática</a>
            <a class="dropdown-item" href="#">Português</a>
            <a class="dropdown-item" href="#">Inglês</a>
          </div>
        </li>
      </ul>
    </div>
    
    
    <form class=" form-inline my-1 lg-0 text-white">
       <input class="form-control mr-sm-2" type="search text-white" placeholder="Pesquisar..." aria-label="Pesquisar">
       <button class=" text-white btn btn-outline-dark my-2 my-sm-0 " type="submit  ">Pesquisar </button>
     </form>
    </nav> 
    <br><br> 
    <div class="container">
   <div class="jumbotron jumbotron-fluid">
     <div class="row">
       <div class="col-12 text-center my-1">
         <h1 class="display-5"><i class="fa fa-cogs text-primary" aria-hidden="true"></i> Cadastro - Funcionários<h1>
         </div>
       </div>
     </div>
   </div>
   

  
  <div id="area">
      <form id="Formulário" autocomplete="off">
        <fieldset>
          <legend text-primary>Cadastro</legend>
          <label>Nome: </label><input class="campo_nome" type="text">
          <label> CPF:</label><input class="campo_cpf" type="password" oninput=mascara(this, 'cpf') id="campo4" type="text" class="form-control" placeholder="Ex.: xxx.xxx.xxx-xx" autocomplete="off" name="customer['cpf']" ><br>
          <label >Cep:</label><input class="campo_CEP" type="text" oninput=mascara(this, 'cep') id="campo6" type="text" class="form-control" placeholder="Ex.: xxxxx-xxx" autocomplete="off" name="customer['cep']"><br>
          Estado:<select name="estado"> 
 		<option value="estado">Selecione o Estado</option> 
 		<option value="ac">Acre</option> 
 		<option value="al">Alagoas</option> 
 		<option value="am">Amazonas</option> 
 		<option value="ap">Amapá</option> 
 		<option value="ba">Bahia</option> 
 		<option value="ce">Ceará</option> 
 		<option value="df">Distrito Federal</option> 
 		<option value="es">Espírito Santo</option> 
 		<option value="go">Goiás</option> 
 		<option value="ma">Maranhão</option> 
 		<option value="mt">Mato Grosso</option> 
 		<option value="ms">Mato Grosso do Sul</option> 
 		<option value="mg">Minas Gerais</option> 
 		<option value="pa">Pará</option> 
 		<option value="pb">Paraíba</option> 
 		<option value="pr">Paraná</option> 
 		<option value="pe">Pernambuco</option> 
 		<option value="pi">Piauí</option> 
 		<option value="rj">Rio de Janeiro</option> 
 		<option value="rn">Rio Grande do Norte</option> 
 		<option value="ro">Rondônia</option> 
 		<option value="rs">Rio Grande do Sul</option> 
 		<option value="rr">Roraima</option> 
 		<option value="sc">Santa Catarina</option> 
 		<option value="se">Sergipe</option> 
 		<option value="sp">São Paulo</option> 
 		<option value="to">Tocantins</option> 
 	</select>
         <label>Rua:</label><input class="campo_rua" type="text">
         <label>Número:</label><input class="campo_Numero" type="text">
         <label>Bairro:</label><input class="campo_Bairro" type="text"><br>
         <label>Cidade:</label><input class="campo_Cidade" type="text"><br>
         <label>Email:</label><input class="campo_Email" type="text" placeholder="Ex:seuemail.tiririca@gmail.com"><br>
          <button type="button" class="btn btn-primary">Enviar</button>
        </fieldset>
      </form>
    </div>
</div>


    <div class="container">
      <div class="row">
        <div class="col-12 mb-3"><br></div>
        
        <div Class="col-sm-4">
          <h3 class="text text-center">Turma TII02</h3>
          <div align="justify"> Segunda turma em técnico de informática para internet do senai Uberaba</div>
        </div>
      
        <div Class="col-sm-4">
          <h3 class="text text-center">Menu</h3>
          <div class="btn-group-vertical btn-block btn-group-lg" role="group">
            <a class="btn btn-outline-primary" href"#">
              Inicio
            </a>
            <a class="btn btn-outline-primary" href"#">
              Empresa
            </a>
            <a class="btn btn-outline-primary" href"#">
              Login
            </a>
            <a class="btn btn-outline-primary" href"#">
              Alunos
            </a>
          </div>
        </div>
        
        <div Class="col-sm-4">
          <h3 class="text text-center">Social Media</h3>
          <div class="btn-group-vertical btn-block btn-group-lg" role="group">
          <a class="btn btn-outline-primary" href"#">
            <i class="fa fa-facebook" aria-hidden="True"></i>
            Facebook
          </a>
          <a class="btn btn-outline-primary" href"#">
            <i class="fa fa-twitter-square" aria-hidden="True"></i>
            Twitter
          </a>
          <a class="btn btn-outline-primary" href"#">
              <i class="fa fa-instagram" aria-hidden="True"></i>
           Instagram
          </a>
          <a class="btn btn-outline-primary" href"#">  
            <i class="fa fa-whatsapp" aria-hidden="True"></i>
            Whatssap
          </a>
        </div>
      </div>
    </div>
       <div class"col-12 mt-5">
         <blockquote classs="blockquote text-center">
         <center><i class="fa fa-copyright " aria-hidden="true" ></i> All rights reserved - 2021</center>
       </blockquote>
      </div>
    </div>

<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
     <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
</body>
