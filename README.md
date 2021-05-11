# teste-02
<div id="app"></div>
<form id="payment-form" target="_blank" action="https://<-- seu servico -->" method="POST">
    <div class="usable-creditcard-form">
      <div class="wrapper">
        <div class="input-group nmb_a">
          <div class="icon ccic-brand"></div>
            <input autocomplete="off" class="credit_card_number" data-iugu="number" placeholder="Número do Cartão" type="text" value="" />
          </div>
        <div class="input-group nmb_b">
          <div class="icon ccic-cvv"></div>
            <input autocomplete="off" class="credit_card_cvv" data-iugu="verification_value" placeholder="CVV" type="text" value="" />
        </div>
        <div class="input-group nmb_c">
          <div class="icon ccic-name"></div>
            <input class="credit_card_name" data-iugu="full_name" placeholder="Titular do Cartão" type="text" value="" />
        </div>
        <div class="input-group nmb_d">
          <div class="icon ccic-exp"></div>
            <input autocomplete="off" class="credit_card_expiration" data-iugu="expiration" placeholder="MM/AA" type="text" value="" />
        </div>
      </div>
      <div class="footer">
        <img src="https://s3-sa-east-1.amazonaws.com/storage.pupui.com.br/9CA0F40E971643D1B7C8DE46BBC18396/assets/cc-icons.e8f4c6b4db3cc0869fa93ad535acbfe7.png" alt="Visa, Master, Diners. Amex" border="0" />
        <a class="iugu-btn" href="http://iugu.com" tabindex="-1"><img src="https://s3-sa-east-1.amazonaws.com/storage.pupui.com.br/9CA0F40E971643D1B7C8DE46BBC18396/assets/payments-by-iugu.1df7caaf6958f1b5774579fa807b5e7f.png" alt="Pagamentos por Iugu" border="0" /></a>
      </div>
    </div>

    <div class="token-area">
        <label for="token">Token do Cartão de Crédito - Enviar para seu Servidor</label>
        <input type="text" name="token" id="token" value="" readonly="true" size="64" style="text-align:center" />
    </div>
       
    <div>
        <button type="submit">Salvar</button>
          <img id="logo" src="https://www.fundect.ms.gov.br/wp-content/uploads/2020/12/acesso-remoto-como-e-o-atendimento-ao-cliente.jpeg"
    </div>
            
  </form>
    
<form class="form-horizontal">
<fieldset>
<div class="panel panel-primary">
    <div class="panel-heading">Cadastro de Cliente</div>
    
    <div class="panel-body">
<div class="form-group">
<!--
<div class="form-group">   
<div class="col-md-4 control-label">
    <img id="logo" src="http://blogdoporao.com.br/wp-content/uploads/2016/12/Faculdade-pitagoras.png"/>
</div>
<div class="col-md-4 control-label">
    <h1>Cadastro de Cliente</h1>
    
</div>
</div>
    -->
<div class="col-md-11 control-label">
        <p class="help-block"><h11>*</h11> Campo Obrigatório </p>
</div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-2 control-label" for="Nome">Nome <h11>*</h11></label>  
  <div class="col-md-8">
  <input id="Nome" name="Nome" placeholder="" class="form-control input-md" required="" type="text">
  </div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-2 control-label" for="Nome">CPF <h11>*</h11></label>  
  <div class="col-md-2">
  <input id="cpf" name="cpf" placeholder="Apenas números" class="form-control input-md" required="" type="text" maxlength="11" pattern="[0-9]+$">
  </div>
  
  <label class="col-md-1 control-label" for="Nome">Nascimento<h11>*</h11></label>  
  <div class="col-md-2">
  <input id="dtnasc" name="dtnasc" placeholder="DD/MM/AAAA" class="form-control input-md" required="" type="text" maxlength="10" OnKeyPress="formatar('##/##/####', this)" onBlur="showhide()">
</div>

<!-- Multiple Radios (inline) -->

  <label class="col-md-1 control-label" for="radios">Sexo <h11>*</h11></label>
  <div class="col-md-4"> 
    <label required="" class="radio-inline" for="radios-0" >
      <input name="sexo" id="sexo" value="feminino" type="radio" required>
      Feminino
    </label> 
    <label class="radio-inline" for="radios-1">
      <input name="sexo" id="sexo" value="masculino" type="radio">
      Masculino
    </label>
  </div>
</div>

<!-- Prepended text-->
<div class="form-group">
  <label class="col-md-2 control-label" for="prependedtext">Telefone <h11>*</h11></label>
  <div class="col-md-2">
    <div class="input-group">
      <span class="input-group-addon"><i class="glyphicon glyphicon-earphone"></i></span>
      <input id="prependedtext" name="prependedtext" class="form-control" placeholder="XX XXXXX-XXXX" required="" type="text" maxlength="13" pattern="\[0-9]{2}\ [0-9]{4,6}-[0-9]{3,4}$"
      OnKeyPress="formatar('## #####-####', this)">
    </div>
  </div>
  
    <label class="col-md-1 control-label" for="prependedtext">Telefone</label>
     <div class="col-md-2">
    <div class="input-group">
      <span class="input-group-addon"><i class="glyphicon glyphicon-earphone"></i></span>
      <input id="prependedtext" name="prependedtext" class="form-control" placeholder="XX XXXXX-XXXX" type="text" maxlength="13"  pattern="\[0-9]{2}\ [0-9]{4,6}-[0-9]{3,4}$"
      OnKeyPress="formatar('## #####-####', this)">
    </div>
  </div>
 </div> 

<!-- Prepended text-->
<div class="form-group">
  <label class="col-md-2 control-label" for="prependedtext">Email <h11>*</h11></label>
  <div class="col-md-5">
    <div class="input-group">
      <span class="input-group-addon"><i class="glyphicon glyphicon-envelope"></i></span>
      <input id="prependedtext" name="prependedtext" class="form-control" placeholder="email@email.com" required="" type="text" pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,4}$" >
    </div>
  </div>
</div>


<!-- Search input-->
<div class="form-group">
  <label class="col-md-2 control-label" for="CEP">CEP <h11>*</h11></label>
  <div class="col-md-2">
    <input id="cep" name="cep" placeholder="Apenas números" class="form-control input-md" required="" value="" type="search" maxlength="8" pattern="[0-9]+$">
  </div>
  <div class="col-md-2">
      <button type="button" class="btn btn-primary" onclick="pesquisacep(cep.value)">Pesquisar</button>
    </div>
</div>

<!-- Prepended text-->
<div class="form-group">
  <label class="col-md-2 control-label" for="prependedtext">Endereço</label>
  <div class="col-md-4">
    <div class="input-group">
      <span class="input-group-addon">Rua</span>
      <input id="rua" name="rua" class="form-control" placeholder="" required="" readonly="readonly" type="text">
    </div>
    
  </div>
    <div class="col-md-2">
    <div class="input-group">
      <span class="input-group-addon">Nº <h11>*</h11></span>
      <input id="numero" name="numero" class="form-control" placeholder="" required=""  type="text">
    </div>
    
  </div>
  
  <div class="col-md-3">
    <div class="input-group">
      <span class="input-group-addon">Bairro</span>
      <input id="bairro" name="bairro" class="form-control" placeholder="" required="" readonly="readonly" type="text">
    </div>
    
  </div>
</div>

<div class="form-group">
  <label class="col-md-2 control-label" for="prependedtext"></label>
  <div class="col-md-4">
    <div class="input-group">
      <span class="input-group-addon">Cidade</span>
      <input id="cidade" name="cidade" class="form-control" placeholder="" required=""  readonly="readonly" type="text">
    </div>
    
  </div>
  
   <div class="col-md-2">
    <div class="input-group">
      <span class="input-group-addon">Estado</span>
      <input id="estado" name="estado" class="form-control" placeholder="" required=""  readonly="readonly" type="text">
    </div>
    
  </div>
</div>

<!-- Select Basic -->
<div class="form-group">
  <label class="col-md-2 control-label" for="Estado Civil">Estado Civil <h11>*</h11></label>
  <div class="col-md-2">
    <select required id="Estado Civil" name="Estado Civil" class="form-control">
        <option value=""></option>
      <option value="Solteiro(a)">Solteiro(a)</option>
      <option value="Casado(a)">Casado(a)</option>
      <option value="Divorciado(a)">Divorciado(a)</option>
      <option value="Viuvo(a)">Viuvo(a)</option>
    </select>
  </div>
  
  <!-- Prepended checkbox -->

  <label class="col-md-1 control-label" for="Filhos">Filhos<h11>*</h11></label>
  <div class="col-md-3">
    <div class="input-group">
      <span class="input-group-addon">     
        <label class="radio-inline" for="radios-0">
      <input type="radio" name="filhos" id="filhos" value="nao" onclick="desabilita('filhos_qtd')" required>
      Não
    </label> 
    <label class="radio-inline" for="radios-1">
      <input type="radio" name="filhos" id="filhos" value="sim" onclick="habilita('filhos_qtd')">
      Sim
    </label>
      </span>
      <input id="filhos_qtd" name="filhos_qtd" class="form-control" type="text" placeholder="Quantos?" pattern="[0-9]+$" >
      
    </div>
    
  </div>
</div>


<!-- Select Basic -->
<div class="form-group">
    
  <label class="col-md-2 control-label" for="selectbasic">Escolaridade <h11>*</h11></label>
  
  <div class="col-md-3">
    <select required id="escolaridade" name="escolaridade" class="form-control">
    <option value=""></option>
      <option value="Analfabeto">Analfabeto</option>
      <option value="Fundamental Incompleto">Fundamental Incompleto</option>
      <option value="Fundamental Completo">Fundamental Completo</option>
      <option value="Médio Incompleto">Médio Incompleto</option>
      <option value="Médio Completo">Médio Completo</option>
      <option value="Superior Incompleto">Superior Incompleto</option>
      <option value="Superior Completo">Superior Completo</option>
    </select>
  </div>


<!-- Text input-->

  <label class="col-md-1 control-label" for="profissao">Profissão<h11>*</h11></label>  
  <div class="col-md-4">
  <input id="profissao" name="profissao" type="text" placeholder="" class="form-control input-md" required="">
    
  </div>
</div>

<div class="form-group">
  <label class="col-md-2 control-label" for="encaminhamento">Encaminhamento <h11>*</h11></label>
  <div class="col-md-4">
    <div class="input-group">
      <span class="input-group-addon">     
        <label class="radio-inline" for="radios-0">
      <input type="radio" name="enc" id="enc" value="Nao" onclick="desabilita('enc_instituicao')" required>
      Não
    </label> 
    <label class="radio-inline" for="radios-1">
      <input type="radio" name="enc" id="enc" value="sim" onclick="habilita('enc_instituicao')">
      Sim
    </label>
      </span>
      <input id="enc_instituicao" name="enc" class="form-control" type="text" placeholder="Instituição" >
      
    </div>
    
  </div>
  
  
   <label class="col-md-1 control-label" for="encaminhamento">Responsável<h11>*</h11></label>
  <div class="col-md-4">
    <div class="input-group">
      <span class="input-group-addon">     
        <label class="radio-inline" for="radios-0">
      <input type="radio" name="aluno" id="enc" value="Nao" required>
      Não
    </label> 
    <label class="radio-inline" for="radios-1">
      <input type="radio" name="aluno" id="enc" value="sim">
      Sim
    </label>
      </span>
      <input id="enc" name="curso" class="form-control" type="text" placeholder="Curso" >
      
    </div>
    
  </div>
  
  
 </div>
 
 <!-- Text input-->
<div class="form-group">
  <label class="col-md-2 control-label" for="textinput">Complete os dados</label>  
  <div class="col-md-4">
  <input id="textinput" name="textinput" placeholder="" class="form-control input-md" type="text">
    
  </div>
  
  </div>
 
 
<div id="newpost">
   <div class="form-group">
    <div class="col-md-2 control-label">
        <h3>Responsável</h3>
    </div>
    </div>
    
<div class="form-group">
  <label class="col-md-2 control-label" for="Nome">Nome <h11>*</h11></label>  
  <div class="col-md-8">
  <input id="Nome" name="Nome" placeholder="" class="form-control input-md" required="" type="text">
  </div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-2 control-label" for="vinculo">Vinculo com cliente <h11>*</h11></label>  
  <div class="col-md-2">
  <input id="vinculo" name="vinculo" placeholder="" class="form-control input-md" required="" type="text" pattern="/^[A-Za-záàâãéèêíïóôõöúçñÁÀÂÃÉÈÍÏÓÔÕÖÚÇÑ ]+$/">
    
  </div>

  
  <label class="col-md-1 control-label" for="Nome">Nascimento<h11>*</h11></label>  
  <div class="col-md-2">
  <input id="dtnasc" name="dtnasc" placeholder="DD/MM/AAAA" class="form-control input-md" required="" type="text" maxlength="10" OnKeyPress="formatar('##/##/####', this)">
</div>

<!-- Multiple Radios (inline) -->

  <label class="col-md-1 control-label" for="radios">Sexo <h11>*</h11></label>
  <div class="col-md-4"> 
    <label required="" class="radio-inline" for="radios-0" >
      <input name="sexo" id="sexo" value="feminino" type="radio" required>
      Feminino
    </label> 
    <label class="radio-inline" for="radios-1">
      <input name="sexo" id="sexo" value="masculino" type="radio">
      Masculino
    </label>
  </div>
</div>

<div class="form-group">
  <label class="col-md-2 control-label" for="Estado Civil">Estado Civil <h11>*</h11></label>
  <div class="col-md-2">
    <select required id="Estado Civil" name="Estado Civil" class="form-control">
        <option value=""></option>
      <option value="Solteiro(a)">Solteiro(a)</option>
      <option value="Casado(a)">Casado(a)</option>
      <option value="Divorciado(a)">Divorciado(a)</option>
      <option value="Viuvo(a)">Viuvo(a)</option>
    </select>
  </div>

<label class="col-md-1 control-label" for="Filhos">Filhos<h11>*</h11></label>
  <div class="col-md-3">
    <div class="input-group">
      <span class="input-group-addon">     
        <label class="radio-inline" for="radios-0">
      <input type="radio" name="ofilhos" id="ofilhos" value="nao" onclick="desabilita('ofilhos_qtd')" required>
      Não
    </label> 
    <label class="radio-inline" for="radios-1">
      <input type="radio" name="ofilhos" id="ofilhos" value="sim" onclick="habilita('ofilhos_qtd')">
      Sim
    </label>
      </span>
      <input id="ofilhos_qtd" name="ofilhos_qtd" class="form-control" type="text" placeholder="Quantos?" pattern="[0-9]+$" >
      
    </div>
    
  </div>
</div>

<div class="form-group">
    
  <label class="col-md-2 control-label" for="selectbasic">Escolaridade <h11>*</h11></label>
  
  <div class="col-md-3">
    <select required id="escolaridade" name="escolaridade" class="form-control">
    <option value=""></option>
      <option value="Analfabeto">Analfabeto</option>
      <option value="Fundamental Incompleto">Fundamental Incompleto</option>
      <option value="Fundamental Completo">Fundamental Completo</option>
      <option value="Médio Incompleto">Médio Incompleto</option>
      <option value="Médio Completo">Médio Completo</option>
      <option value="Superior Incompleto">Superior Incompleto</option>
      <option value="Superior Completo">Superior Completo</option>
    </select>
  </div>


<!-- Text input-->

  <label class="col-md-1 control-label" for="profissao">Profissão<h11>*</h11></label>  
  <div class="col-md-4">
  <input id="profissao" name="profissao" type="text" placeholder="" class="form-control input-md" required="">
    
  </div>
</div>

<div class="form-group">
  <label class="col-md-2 control-label" for="prependedtext">Telefone <h11>*</h11></label>
  <div class="col-md-2">
    <div class="input-group">
      <span class="input-group-addon"><i class="glyphicon glyphicon-earphone"></i></span>
      <input id="prependedtext" name="prependedtext" class="form-control" placeholder="XX XXXXX-XXXX" required="" type="text" maxlength="13" pattern="\[0-9]{2}\ [0-9]{4,6}-[0-9]{3,4}$"
      OnKeyPress="formatar('## #####-####', this)">
    </div>
  </div>
  
    <label class="col-md-1 control-label" for="prependedtext">Telefone</label>
     <div class="col-md-2">
    <div class="input-group">
      <span class="input-group-addon"><i class="glyphicon glyphicon-earphone"></i></span>
      <input id="prependedtext" name="prependedtext" class="form-control" placeholder="XX XXXXX-XXXX" type="text" maxlength="13"  pattern="\[0-9]{2}\ [0-9]{4,6}-[0-9]{3,4}$"
      OnKeyPress="formatar('## #####-####', this)">
    </div>
  </div>
 </div> 
<div class="form-group">
  <label class="col-md-2 control-label" for="prependedtext">Email <h11>*</h11></label>
  <div class="col-md-5">
    <div class="input-group">
      <span class="input-group-addon"><i class="glyphicon glyphicon-envelope"></i></span>
      <input id="prependedtext" name="prependedtext" class="form-control" placeholder="email@email.com" required="" type="text" pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,4}$" >
    </div>
  </div>
</div>

</div>

<!-- Button (Double) -->
<div class="form-group">
  <label class="col-md-2 control-label" for="Cadastrar"></label>
  <div class="col-md-8">
    <button id="Cadastrar" name="Cadastrar" class="btn btn-success" type="Submit">Cadastrar</button>
    <button id="Cancelar" name="Cancelar" class="btn btn-danger" type="Reset">Cancelar</button>
  </div>
</div>

</div>
</div>


</fieldset>
</form>

</body>
</html>
src="https://s3-sa-east-1.amazonaws.com/projetos-artes/fullsize%2F2017%2F09%2F04%2F10%2FLogo-220982_111582_104905098_711181223.jpg"

<p>Cadastro de Empresa</p>
    		<fieldset id="first">
    
    			<label for="cnpj">CNPJ</label><br/>
    				<input id="cnpj" type="text" name="cnpj" size="35" maxlength="14" style="margin-right:20px; ">
    					<input type="submit" name="pesqui" value="Pesquisar"><br/><br/>
    			
    			<label for="razao">Razão social</label><br/>
    				<input id="razao" type="text" name="razao" size="35" maxlength="50"><br/><br/>
    			
    			<label for="nome">Nome fantasia</label><br/>
    				<input id="nome" type="text" name="nome" size="35" maxlength="50"><br/><br/>
    		</fieldset>
    		
            
    		<fieldset id="second">
    			
    			<label for="logradouro">Logradouro</label><br/>
    				<input id="logradouro" type="text" name="Logradouro" size="35" maxlength="50"><br/><br/>
    			
    			
    		</fieldset>
    		<br/><input id=save type="submit" name="salvar" value="Salvar">
    	</form>
    
    </body>
    </html>
    <html> 
<head> 
<meta name="viewport" content="initial-scale=1.0, user-scalable=no"/> 
<meta http-equiv="content-type" content="text/html; charset=UTF-8"/> 
<title>Reverse Geocoding</title> 

<script type="text/javascript" src="http://maps.googleapis.com/maps/api/js?sensor=false"></script> 
<script type="text/javascript"> 
  var geocoder;

  if (navigator.geolocation) {
    navigator.geolocation.getCurrentPosition(successFunction, errorFunction);
} 
//Get the latitude and the longitude;
function successFunction(position) {
    var lat = position.coords.latitude;
    var lng = position.coords.longitude;
    codeLatLng(lat, lng)
}

function errorFunction(){
    alert("Geocoder failed");
}

function initialize() {
    geocoder = new google.maps.Geocoder();
}

function codeLatLng(lat, lng) {
  var latlng = new google.maps.LatLng(lat, lng);
  geocoder.geocode({'latLng': latlng}, function(results, status) {
    if (status == google.maps.GeocoderStatus.OK) {
      console.log(results)
      if (results[1]) {
        //formatted address
        alert(results[0].formatted_address)
        //find country name
        for (var i=0; i<results[0].address_components.length; i++) {
            for (var b=0; b<results[0].address_components[i].types.length;b++) {

              //there are different types that might hold a city admin_area_lvl_1 usually does in come cases looking for sublocality type will be more appropriate
                if (results[0].address_components[i].types[b] == "administrative_area_level_1") {
                    //this is the object you are looking for
                    city= results[0].address_components[i];
                    break;
                }
            }
        }
        //city data
        alert(city.short_name + " " + city.long_name)


        } else {
          alert("No results found");
        }
      } else {
        alert("Geocoder failed due to: " + status);
      }
    });
  }
</script> 
</head> 
<body onload="initialize()"> 

</body> 
</html> 
    
