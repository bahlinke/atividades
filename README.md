<html>
<head>
<title> Formulário Padrão HTML SEM JavaScript </title>
</head>
<head>
<title> Formulário Padrão HTML COM JavaScript </title>
<script>
nome1=window.prompt("Qual seu nome?");
if (nome1!=null && nome1!="")
{
document.write("Olá, "+nome1+"!");
}
else
{
document.write("Olá, visitante!");
}
</script>
<body>
<script>
function validar()
{
if (document.cadastro.nome.value == "")
{ window.alert("Você deve preencher o campo Nome.");
document.cadastro.nome.focus();
return false;
}
if (document.cadastro.observacoes.value == "")
{ window.alert("Você deve colocar alguma observação...");
document.cadastro.observacoes.focus();
return false;
}
}
<INPUT TYPE="SUBMIT" VALUE="Enviar os dados" onClick="validar();">
</script>
</head>
<body>
<FORM ACTION="mailto:teste@gmail.com" METHOD="POST" ENCTYPE="text/plain"
NAME="cadastro">
<p> Por favor, preencha os campos abaixo e depois clique no botão Enviar. Caso
necessite apagar os dados, dê um clique no botão Limpar.<br> Muito Obrigado!
<br><br><br></p>
Nome Completo: <INPUT TYPE="TEXT" NAME="nome" SIZE="35">
Seu e-mail: <INPUT TYPE="TEXT" NAME="email" SIZE="35"> <br>
Sexo:<br>
<INPUT TYPE="RADIO" NAME="sexo" VALUE="f"> Feminino <br>
<INPUT TYPE="RADIO" NAME="sexo" VALUE="m"> Masculino <br><br>
Estado Civil:<br>
<INPUT TYPE="RADIO" NAME="civil" VALUE="s"> Solteiro <br>
<INPUT TYPE="RADIO" NAME="civil" VALUE="c"> Casado <br>
<INPUT TYPE="RADIO" NAME="civil" VALUE="e"> Enrolado <br><br>
Bens que possui:<br>
<INPUT TYPE="CHECKBOX" NAME="bens" VALUE="c"> Casa <br>
<INPUT TYPE="CHECKBOX" NAME="bens" VALUE="a"> Automovel <br>
<INPUT TYPE="CHECKBOX" NAME="bens" VALUE="m"> Moto <br><br>
Faixa de idade: <SELECT NAME="faixaidade">
<OPTION VALUE="3a10"> 3 a 10 anos
<OPTION VALUE="11a25"> 11 a 25 anos
<OPTION VALUE="26a35"> 26 a 35 anos
<OPTION VALUE="36a55"> 36 a 55 anos
<OPTION VALUE="56a90"> 56 a 90 anos
</SELECT>
Hobby preferido: <SELECT NAME="hobby">
<OPTION VALUE="livros"> Ler livros
<OPTION VALUE="musica"> Ouvir música
<OPTION VALUE="cinema"> Assistir filmes
<OPTION VALUE="esporte"> Praticar esportes
<OPTION VALUE="games"> Jogar games
</SELECT><br><br>
Observações Gerais:<br>
<TEXTAREA NAME="observacoes" ROWS="5" COLS="60"></TEXTAREA><br>
<INPUT TYPE="SUBMIT" VALUE="Enviar os dados">
<INPUT TYPE="RESET" VALUE="Limpar os dados">
</FORM>
</body>
</html>
