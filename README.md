# Formulario
atividade da lista de exercicio
<!DOCTYPE html>

<html>
<h1>Formulário</h1>
  <form action="/action_page.php">
    <fieldset>
      <legend>Dados Pessoais:</legend>
  
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title> Lista de Exercicio 1 </title>
</head>

<body>
  
  <form action="/action_page.php" method="post">
    <label><br>Nome</br></label>
    <input type="text" value="" required/>
    <label><br>Data de Nascimento</br></label>
    <input type="date" value="">
    <label><br>Endereço</br></label>
    <input type="text" value="" required/>
    <label><br>Bairro</br></label>
    <input type="text" value="" required/> 
    <label><br>Cidade</br></label>
    <input type="text" value="" required/>
    <label><br>CEP</br></label>
    <input type="number" value="" required/>
     <label for="estado">Estado:</label>
  <select id="" name="estado">
    <option value="ceará" selected> Ceará </option>
    <option value="Piauí">Piauí</option>
    <option value="Bahia">Bahia</option>
    <option value="Acre">Acre</option>
    </select>
    
      </fieldset>
     <fieldset>
      <legend>Dados Profissionais:</legend>
  <br>
    <h13> Natureza do Cargo</hr13>
      <br>
  <label for="Gerência">Gerência</label>
  <input type="radio" id="ger" name="nat_cargo" value="Gerência">
  <label for="Financeiro">Financeiro</label>
  <input type="radio" id="fin" name="nat_cargo" value="Financeiro">
  <label for="Recepção">Recepção</label>
  <input type="radio" id="Rec" name="nat_cargo" value="Recepção">
  <label for="Administrativo">Administrativo</label>
  <input type="radio" id="Adm" name="nat_cargo" value="Administrativo">
 <label for="Juridico">Juridico</label>
 <input type="radio" id="jur" name="nat_cargo" value="Juridico">
    <p> 
      
      <h8> Área de Interesse</h8>
    </p>
    <input type="checkbox" id="com" name="area_interesse" value="Computação">
  <label for="area_interesse">Computação</label>
  <input type="checkbox" id="Quim" name="area_interesse" value="Quimica">
  <label for="area_interesse">Quimica</label>
  <input type="checkbox" id="mei" name="area_interesse" value="Meio Ambiente">
  <label for="area_interesse">Meio Ambiente</label>
  <input type="checkbox" id="en" name="area_interesse" value="Engenharia">
  <label for="area_interesse">Engenharia</label>
  <input type="checkbox" id="mat" name="area_interesse" value="Matemática">
  <label for="area_interesse">Matemática</label>

    <h5>Mini-Currículo:</h5>
       <textarea name="message" rows="10" cols="30">
</textarea> 
    </fieldset>
    <input tyoe="reset" value="Limpar">
    <input type="submit" value="Enviar">
    
</form> 
      
    <!-- Code injected by live-server -->
<script>
	// <![CDATA[  <-- For SVG support
	if ('WebSocket' in window) {
		(function () {
			function refreshCSS() {
				var sheets = [].slice.call(document.getElementsByTagName("link"));
				var head = document.getElementsByTagName("head")[0];
				for (var i = 0; i < sheets.length; ++i) {
					var elem = sheets[i];
					var parent = elem.parentElement || head;
					parent.removeChild(elem);
					var rel = elem.rel;
					if (elem.href && typeof rel != "string" || rel.length == 0 || rel.toLowerCase() == "stylesheet") {
						var url = elem.href.replace(/(&|\?)_cacheOverride=\d+/, '');
						elem.href = url + (url.indexOf('?') >= 0 ? '&' : '?') + '_cacheOverride=' + (new Date().valueOf());
					}
					parent.appendChild(elem);
				}
			}
			var protocol = window.location.protocol === 'http:' ? 'ws://' : 'wss://';
			var address = protocol + window.location.host + window.location.pathname + '/ws';
			var socket = new WebSocket(address);
			socket.onmessage = function (msg) {
				if (msg.data == 'reload') window.location.reload();
				else if (msg.data == 'refreshcss') refreshCSS();
			};
			if (sessionStorage && !sessionStorage.getItem('IsThisFirstTime_Log_From_LiveServer')) {
				console.log('Live reload enabled.');
				sessionStorage.setItem('IsThisFirstTime_Log_From_LiveServer', true);
			}
		})();
	}
	else {
		console.error('Upgrade your browser. This Browser is NOT supported WebSocket for Live-Reloading.');
	}
	// ]]>
</script>
</body>
  </html>
