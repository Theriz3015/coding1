
## usando else/else if para tomar decisões

```.js
let decisao = prompt("Escolha: 1 para Consulta ,2 para entrar em contato ,3 para Cancelar")


if (decisao == 1) {
  let cpf = prompt("digite seu CPF")
  window.alert("Sua consulta foi realizada.")
  console.log("Sua consulta foi realizada.")
} else if (decisao == 2) {
console.log("Entre em contato 818457-9764");
} else if (decisao == 3) {
  console.log("Atendimento Cancelado");
} else {
  window.alert("Atendimento Cancelado")
  console.log("Atendimento Cancelado")
}
                              // usando if e else if //

let nome = prompt("Qual o seu nome?").toLowerCase();
let senha = prompt("Digite a sua senha:").toLowerCase();

window.alert(`Seu nome: ${nome} 
Sua senha: ${senha}`);

let pesquisa = prompt("Pesquise os preços de nossas opções: pizza de pepperoni, assinha de frango, milk shake, coxinha, refrigerante");

switch (pesquisa) {
  case "pizza de pepperoni":
    console.log(`Olá ${nome} a pizza de pepperoni custa R$30,00`)
    break;
  case "asinha de frango":
console.log(nome +  " a assinha de frango custa R$15,00")
break;
  case "milkshake":
    console.log(nome +  " o milk shake custa R$12,00")
    break;
  case "refrigerante":
    console.log(nome + " o refrigerante custa R$5,00")
    break;
  case "coxinha":
    console.log(nome + " a coxinha custa R$5,00")
    break;
    default:
    console.log(" Não foi possível realizar a pesquisa");
      window.alert("Não foi possível realizar a pesquisa")
      }
                         //usando case switch//

let nome = prompt("Qual o seu nome?").toLowerCase();
let senha = prompt("Digite a sua senha:").toLowerCase();

window.alert(`Seu nome: ${nome} 
Sua senha: ${senha}`);

let pesquisa = prompt("Pesquise os preços de nossas opções: pizza de pepperoni, assinha de frango, milk shake, coxinha, refrigerante");

switch (pesquisa) {
  case "pizza de pepperoni":
    console.log(`Olá ${nome} a pizza de pepperoni custa R$30,00`)
    break;
  case "asinha de frango":
console.log(nome +  " a assinha de frango custa R$15,00")
break;
  case "milkshake":
    console.log(nome +  " o milk shake custa R$12,00")
    break;
  case "refrigerante":
    console.log(nome + " o refrigerante custa R$5,00")
    break;
  case "coxinha":
    console.log(nome + " a coxinha custa R$5,00")
    break;
    default:
    console.log(" Não foi possível realizar a pesquisa");
      window.alert("Não foi possível realizar a pesquisa")
      }
```
