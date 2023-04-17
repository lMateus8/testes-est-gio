# testes-estágio
Aqui você encontrará os resultados dos testes de estágio da Target
# Soluções : Questões 2 a 5
_____________________________________________________________________________________________________
# 2 - Sequência de Fibonacci
  function fibonacci(n) {
    if (n <= 0) {
      return null;
    } else if (n === 1) {
      return [0];
    } else if (n === 2) {
      return [0, 1];
    } else {
      const fib = [0, 1];
      while (fib.length < n) {
        const nextNum = fib[fib.length - 1] + fib[fib.length - 2];
        fib.push(nextNum);
      }
      return fib;
    }
  }
  
  // Número a ser verificado
  const numero = 21;
  
  // Chama a função para calcular a sequência de Fibonacci
  const sequenciaFibonacci = fibonacci(numero);
  
  // Verifica se o número pertence à sequência de Fibonacci
  if (sequenciaFibonacci.includes(numero)) {
    console.log(`O número ${numero} pertence à sequência de Fibonacci.`);
  } else {
    console.log(`O número ${numero} não pertence à sequência de Fibonacci.`);
  }
  
  ____________________________________________________________________________________________________________
  
  # 4 - Valores de faturamento por estado
  
  // Valores de faturamento por estado
const faturamentoSP = 67836.43;
const faturamentoRJ = 36678.66;
const faturamentoMG = 29229.88;
const faturamentoES = 27165.48;
const faturamentoOutros = 19849.53;

// Cálculo do valor total mensal da distribuidora
const valorTotal = faturamentoSP + faturamentoRJ + faturamentoMG + faturamentoES + faturamentoOutros;

// Cálculo do percentual de representação de cada estado
const percentualSP = (faturamentoSP / valorTotal) * 100;
const percentualRJ = (faturamentoRJ / valorTotal) * 100;
const percentualMG = (faturamentoMG / valorTotal) * 100;
const percentualES = (faturamentoES / valorTotal) * 100;
const percentualOutros = (faturamentoOutros / valorTotal) * 100;

// Exibição dos resultados
console.log(`Percentual de representação de SP: ${percentualSP.toFixed(2)}%`);
console.log(`Percentual de representação de RJ: ${percentualRJ.toFixed(2)}%`);
console.log(`Percentual de representação de MG: ${percentualMG.toFixed(2)}%`);
console.log(`Percentual de representação de ES: ${percentualES.toFixed(2)}%`);
console.log(`Percentual de representação de Outros: ${percentualOutros.toFixed(2)}%`);
_______________________________________________________________________________________________________________________________

  # 5 - Função para inverter os caracteres de uma string
  
  // Função para inverter os caracteres de uma string
function inverterString(str) {
    let resultado = "";
    for (let i = str.length - 1; i >= 0; i--) {
      resultado += str[i];
    }
    return resultado;
  }
  
  // Exemplo de uso da função -- Digite aqui 
  const inputString = "Mateus de Souza Menezes";
  const invertedString = inverterString(inputString);
  console.log(`String original: ${inputString}`);
  console.log(`String invertida: ${invertedString}`);
  
  
  
