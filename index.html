<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<title>Termo de Responsabilidade</title>

<script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>

<style>
body {
  font-family: Arial;
  max-width: 700px;
  margin: auto;
  padding: 20px;
  color: #000;
}

h2 { text-align: center; }

input, textarea {
  border: none;
  border-bottom: 1px solid black;
  width: 100%;
  margin-top: 5px;
}

textarea { height: 60px; }

.row {
  display: flex;
  gap: 30px;
}

.row div { flex: 1; }

.radio-group { display: flex; gap: 20px; margin-top: 10px; }

.check-group label {
  display: block;
  margin-top: 8px;
}

button {
  margin-top: 15px;
  padding: 10px;
  width: 100%;
  background: black;
  color: white;
  border: none;
}
</style>
</head>

<body>

<h2>📝 TERMO DE RESPONSABILIDADE E CONSENTIMENTO - MAQUIAGEM</h2>

<form id="form">

<p><b>Identificação do Cliente:</b></p>
<input type="text" id="nome" required>

<div class="row">
  <div>
    <p><b>Data do Atendimento:</b></p>
    <input type="date" id="data" required>
  </div>

  <div>
    <p><b>Hora:</b></p>
    <input type="time" id="hora" required>
  </div>
</div>

<hr>

<p><b>Saúde e Condições da Pele (Anamnese)</b></p>

<p>
Declaro que fui informado(a) sobre a necessidade de informar alergias a cosméticos (talco, conservantes, fragrâncias etc.).
Declaro que NÃO possuo, ou informei abaixo, alergias, sensibilidades, doenças de pele ativas (acne severa, herpes, dermatite), ou uso de medicamentos fortes (ex: Roacutan).
</p>

<p><b>Campo de Observações / Alergias:</b></p>
<textarea id="alergia"></textarea>

<hr>

<p><b>Responsabilidade do Cliente</b></p>

<p>
Eu <b><span id="p_assinatura"></span></b> comprometo-me a higienizar meu rosto antes do atendimento, caso solicitado pela maquiadora.
Caso haja reação alérgica durante ou após o atendimento, a responsabilidade é isenta à profissional, desde que os produtos utilizados tenham sido acordados ou previamente testados.
</p>

<hr>

<p><b>Consentimento de Imagem</b></p>

<div class="radio-group">
  <label><input type="radio" name="imagem" value="Autoriza"> Autoriza</label>
  <label><input type="radio" name="imagem" value="Não autoriza"> Não autoriza</label>
</div>

<hr>

<p><b>Confirmações:</b></p>
<div class="check-group">
  <label><input type="checkbox" class="check"> Declaro que li e concordo com todas as informações</label>
  <label><input type="checkbox" class="check"> Estou ciente das responsabilidades assumidas</label>
  <label><input type="checkbox" class="check"> Autorizo o procedimento conforme descrito</label>
</div>

<hr>

<p><b>Assinatura do Cliente:</b></p>
<input type="text" id="assinatura" required>

<button type="submit">Gerar Termo</button>

</form>

<!-- PDF (SEM ALTERAR CLÁUSULAS) -->
<div id="pdf" style="display:none; padding:20px; font-family:Arial;">

<h2 style="text-align:center;">TERMO DE RESPONSABILIDADE E CONSENTIMENTO - MAQUIAGEM</h2>

<p><b>Identificação do Cliente:</b> <span id="p_nome"></span></p>

<p><b>Data do Atendimento:</b> <span id="p_data"></span> &nbsp;&nbsp;&nbsp;&nbsp; <b>Hora:</b> <span id="p_hora"></span></p>

<hr>

<p><b>Saúde e Condições da Pele (Anamnese)</b></p>

<p>
Declaro que fui informado(a) sobre a necessidade de informar alergias a cosméticos (talco, conservantes, fragrâncias etc.).
Declaro que NÃO possuo, ou informei abaixo, alergias, sensibilidades, doenças de pele ativas (acne severa, herpes, dermatite), ou uso de medicamentos fortes (ex: Roacutan).
</p>

<p><b>Campo de Observações / Alergias:</b></p>
<p id="p_alergia"></p>

<hr>

<p><b>Responsabilidade do Cliente</b></p>

<p>
Eu <b><span id="p_assinatura_pdf"></span></b> comprometo-me a higienizar meu rosto antes do atendimento, caso solicitado pela maquiadora.
Caso haja reação alérgica durante ou após o atendimento, a responsabilidade é isenta à profissional, desde que os produtos utilizados tenham sido acordados ou previamente testados.
</p>

<hr>

<p><b>Consentimento de Imagem</b></p>

<p>
(<span id="p_imagem"></span>) Autorizo o uso de fotos e vídeos do resultado da maquiagem para fins de portfólio em redes sociais.
</p>

<hr>

<p><b>Confirmações:</b></p>
<ul id="p_checks"></ul>

</div>

<script>
let pdfBlob = null;

document.getElementById("form").addEventListener("submit", async function(e){
e.preventDefault();

const nome = document.getElementById("nome").value;
const data = document.getElementById("data").value;
const hora = document.getElementById("hora").value;
const assinatura = document.getElementById("assinatura").value;
const alergia = document.getElementById("alergia").value;

const imagem = document.querySelector('input[name="imagem"]:checked');
const checks = document.querySelectorAll(".check");

if (!nome || !data || !hora || !assinatura) {
  alert("Preencha todos os campos.");
  return;
}

if (!imagem) {
  alert("Selecione autorização de imagem.");
  return;
}

let ok = true;
checks.forEach(c => { if (!c.checked) ok = false; });

if (!ok) {
  alert("Confirme todas as informações.");
  return;
}

// preencher PDF
document.getElementById("p_nome").innerText = nome;
document.getElementById("p_data").innerText = data;
document.getElementById("p_hora").innerText = hora;
document.getElementById("p_alergia").innerText = alergia || "Nenhuma";
document.getElementById("p_imagem").innerText = imagem.value;
document.getElementById("p_assinatura_pdf").innerText = assinatura;
document.getElementById("p_assinatura").innerText = assinatura;

const lista = document.getElementById("p_checks");
lista.innerHTML = "";

checks.forEach(c => {
  const li = document.createElement("li");
  li.innerText = c.parentElement.innerText.trim();
  lista.appendChild(li);
});

const element = document.getElementById("pdf");
element.style.display = "block";

const worker = html2pdf().from(element).toPdf();

pdfBlob = await worker.outputPdf("blob");

await worker.save();

element.style.display = "none";

/* 🔥 AQUI ESTÁ A MUDANÇA: abre compartilhamento automático */
const file = new File([pdfBlob], "termo.pdf", { type: "application/pdf" });

const mensagem = "Segue o termo de responsabilidade assinado.";

if (navigator.canShare && navigator.canShare({ files: [file] })) {
  await navigator.share({
    title: "Termo de Responsabilidade",
    text: mensagem,
    files: [file]
  });
} else {
  alert("Seu dispositivo não suporta envio direto. Baixe o PDF manualmente.");
}

});
</script>

</body>
</html>
