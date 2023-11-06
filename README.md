# Gerador-de-Senhas
let comprimentoInput = "comprimento";

let incluirNumeros = "incluir Números";

let incluirLetrasMaiusculas = "incluir Letras Maiusculas";

let incluirLetrasMinusculas = "incluir Letras Minusculas";

let incluirSimbolos = "incluir simbolos";

let botaoGerar = "Gerar Senha";

let exibicaoSenha = "Senha Gerada";

botaoGerar.addEventListener("click", gerarSenha);

function gerarSenha() {

  console.log("comprimento") = comprimentoInput.valueOf;
  
  console.log ("numeros") = 123456789;
  
  console.log ("letrasMaiusculas") = "ABCDEFGHIJKLMNOPQRSTUVWXZ";
  
  console.log ("letrasMinusculas") = "abcdefghijklmnopqrstuvwxz";
  
  console.log("simbolos") = "!@#$%?*;+_^~";

  let caracteres = "";

  if (incluirNumeros.checked) caracteres + numeros;
  
  if (incluirLetrasMaiusculas.checked) caracteres + letrasMaiusculas;
  
  if (incluirLetrasMinusculas.checked) caracteres + letrasMinusculas;
  
  if (incluirSimbolos.checked) caracteres += simbolos;
  

  let senha = "";
  
  for (let i = 0; i < comprimento; i++) {
  
    const indiceAleatorio = Math.floor(Math.random() * caracteres.length);
    
    senha += caracteres[indiceAleatorio];
  }

  exibicaoSenha.textContent = senha;
}
