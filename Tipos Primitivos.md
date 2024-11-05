## Tipos Primitivos

```.js
let nome = prompt("Qual é seu nome?");

let idade = prompt("Qual é a sua idade?");

console.log(`Olá meu nome é ${nome} e tenho ${idade} anos`)

/* use /* para transformar em comentário
*/

let cidade = prompt("em qual cidade você mora?")

let nomeDousuario = prompt("Qual seu nome?")

console.log (`Bem-vindo(a) ${nomeDousuario} você mora em ${cidade}`);



let num1 = 10;
let num2 = 5;
console.log ("Soma:", num1 + num2);
console.log ("Subtração", num1 - num2);
console.log ("Multiplicação", num1 * num2);
console.log ("Divisão", num1 / num2);



let base = 10;
let altura = 5;

let area = (base * altura) / 2;

console.log(`A área do triangulo é`, area );



let nota1 = 8;
let nota2 = 6;
let nota3 = 10;
let media = (nota1 + nota2 + nota3) / 3;

console.log(`O resultado da nota é...`, media);



let precoOriginal = prompt("Digite o preço original do produto");
let percentualDesconto = prompt ("Digite o percentual de desconto (ex: 10 para 10%):");
let valorDesconto = (precoOriginal * percentualDesconto) / 100;
let precoFinal = precoOriginal - valorDesconto;
console.log("O valor do desconto é R$", valorDesconto.toFixed(2));
console.log("O preço final do produto é R$", precoFinal.toFixed(2));


// Tabela de alíquotas simplificada (ajuste conforme a legislação vigente)

const tabelaAliquotas = [
    { faixaSalarial: 1903.99, aliquota: 0, deducao: 0 },
    { faixaSalarial: 2826.65, aliquota: 7.5, deducao: 142.80 },
    // ... adicione mais faixas conforme necessário
];

// Solicita o salário bruto ao usuário
const salarioBruto = parseFloat(prompt("Digite o seu salário bruto:"));

// Função para calcular o imposto de renda
function calcularImpostoDeRenda(salarioBruto) {
    let imposto = 0;
    let aliquota = 0;

    // Encontra a faixa salarial correspondente
    for (let i = 0; i < tabelaAliquotas.length; i++) {
        if (salarioBruto <= tabelaAliquotas[i].faixaSalarial) {
            aliquota = tabelaAliquotas[i].aliquota;
            imposto = (salarioBruto * aliquota / 100) - tabelaAliquotas[i].deducao;
            break;
        }
    }

    return { imposto, aliquota };
}

// Chama a função e exibe o resultado
const { imposto, aliquota } = calcularImpostoDeRenda(salarioBruto);

console.log(`Salário bruto: R$ ${salarioBruto.toFixed(2)}`);
console.log(`Alíquota aplicada: ${aliquota}%`);
console.log(`Imposto de renda a pagar: R$ ${imposto.toFixed(2)}`);

 

let dolaratual = 5.71
let realproposto = prompt('Insira o valor em real que você quer converter para dólar: ');
let dolarproposto = prompt('Insira o valor em dolar que você quer converter para real: ');

dolaratual = parseFloat(dolaratual);
realproposto = parseFloat(realproposto);
dolarproposto = parseFloat(dolarproposto);

let realfinal = realproposto / dolaratual;
let dolarfinal = dolarproposto * dolaratual;

let realfinalformatado = realfinal.toFixed(2);
let dolarfinalformatado = dolarfinal.toFixed(2);

console.log(`O seu valor convertido de dólar para real é: ${dolarfinalformatado}`);
console.log(`O seu valor convertido de real para dólar é: ${realfinalformatado}`);



let Celsius = prompt('Digite a temperatura em Celsius: ');
let ConverterF = ((Celsius * 1.8) + 32);
let ConverterFformatado = ConverterF.toFixed(2);

console.log(`O valor da temperatura em Celsius convertido para Fahrenheit: ${ConverterF}`);



let peso = prompt ('Digite seu peso: '); 
let altura = prompt ('Digite sua altura em metros: ');

let imc = peso / (altura * altura);
let imcFormatado = imc.toFixed(2);
console.log(`O seu IMC é: ${imcFormatado}`);

```
