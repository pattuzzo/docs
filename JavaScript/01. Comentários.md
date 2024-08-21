### Comentários

<!-- #### **1. Introdução aos Comentários**
- **Importância dos Comentários**
  - O papel dos comentários na manutenção e compreensão do código.
  - Como comentários ajudam na colaboração e na documentação do código.

- **Quando e Como Comentar**
  - Diretrizes para decidir quando comentar o código.
  - Melhores práticas para escrever comentários úteis e informativos.

#### **2. Tipos de Comentários**
- **Comentários Inline**
  - Uso de comentários na mesma linha do código para explicar trechos específicos.
  - Exemplo e boas práticas para comentários inline.

- **Comentários Multilinha**
  - Uso de comentários que abrangem várias linhas para descrever blocos de código ou logicamente relacionados.
  - Exemplo e boas práticas para comentários multilinha.

#### **3. Desativação de Código**
- **Desativação Temporária de Código**
  - Técnicas para desativar trechos de código temporariamente durante o desenvolvimento e testes.
  - Considerações sobre como evitar a inclusão de código desativado na versão final.

#### **4. Documentação**
- **JSDoc**
  - Introdução ao JSDoc e sua importância para a documentação automatizada.
  - Como usar anotações JSDoc para documentar funções, parâmetros e tipos de dados.
  - Exemplos de tags JSDoc comuns (`@param`, `@returns`, `@example`, etc.).

#### **5. Boas Práticas**
- **Clareza e Concisão**
  - Princípios para escrever comentários claros e concisos.
  - Evitar comentários redundantes e garantir que os comentários realmente ajudem na compreensão do código. -->

### 1. Introdução aos Comentários

#### **Importância dos Comentários**
Os comentários ajudam a tornar o código mais fácil de entender e manter, especialmente quando outras pessoas precisam ler ou modificar o código. Eles explicam o que o código faz e, mais importante, por que ele foi escrito daquela maneira. Isso é crucial em ambientes colaborativos e em projetos a longo prazo.

- **Facilitando a compreensão:** Às vezes, o código em si não é autoexplicativo, e os comentários podem fornecer informações adicionais que ajudam a entender a lógica aplicada.
- **Colaboração:** Comentários permitem que outros desenvolvedores entendam rapidamente o que você fez e como seu código se encaixa no resto do projeto.

##### Exemplo:
```javascript
// Exibe uma mensagem de boas-vindas no console
console.log("Bem-vindo!");
```

Aqui, o comentário deixa claro que a linha de código é responsável por exibir uma mensagem de boas-vindas. Simples e direto ao ponto.

#### **Quando e Como Comentar**
Nem todo código precisa ser comentado, mas quando há algo que não é imediatamente óbvio, ou quando a decisão de usar uma determinada abordagem precisa ser explicada, um comentário pode ser extremamente útil.

- **Quando comentar:**
  - Quando o código é complexo ou envolve uma lógica não trivial.
  - Quando você está tomando uma decisão técnica que não é imediatamente evidente.

- **Melhores práticas:**
  - **Seja claro e objetivo:** Evite comentários que expliquem coisas óbvias. Prefira explicar o propósito ou a motivação por trás de um trecho de código.
  - **Explique o porquê:** Concentre-se em explicar por que algo está sendo feito, não apenas o que está sendo feito.

##### Exemplo:
```javascript
// Define o nome do usuário
let nomeUsuario = "João";
```
O comentário explica que a variável nomeUsuario armazena o nome de um usuário, o que é útil para alguém que está lendo o código pela primeira vez.

---

### 2. Tipos de Comentários

#### **Comentários Inline**
Comentários inline são usados para fornecer pequenas explicações ou notas diretamente ao lado do código ao qual se referem. Eles são úteis para trechos específicos onde o código pode não ser autoexplicativo.

- **Boas práticas:** Mantenha os comentários curtos e relevantes. Use-os apenas quando necessário para esclarecer partes específicas do código.

##### Exemplo:
```javascript
let taxaDesconto = 0.1; // Desconto de 10%
```
Este comentário é simples e direto, indicando que `taxaDesconto` é 10%.

#### **Comentários Multilinha**
Comentários multilinha são usados para descrever blocos maiores de código ou para fornecer uma explicação mais detalhada. Eles são especialmente úteis quando você precisa fornecer contexto sobre como um conjunto de funções ou operações trabalha em conjunto.

##### Exemplo:
```javascript
/*
  Este bloco de código calcula o preço final de um produto
  aplicando um desconto de 10%.
*/
let precoOriginal = 100;
let desconto = 10;
let precoFinal = precoOriginal - desconto;
```
Este exemplo usa um comentário multilinha para descrever o que o bloco de código faz, fornecendo contexto suficiente sem entrar em detalhes excessivos.

---

### 3. Desativação de Código

#### **Desativação Temporária de Código**
Durante o desenvolvimento, pode ser necessário desativar partes do código temporariamente. Isso é útil para testes, depuração ou quando você está experimentando novas implementações sem querer remover permanentemente o código existente.

- **Por que desativar código?**
  Desativar código é uma prática comum durante o desenvolvimento, pois permite que você teste e depure partes específicas do código sem afetar outras áreas do programa. Também pode ser útil quando você está experimentando soluções alternativas, mas não quer perder o código original.

- **Como desativar código?**
  Para desativar o código em JavaScript, você pode simplesmente comentar as linhas que deseja desativar. Isso impede que o JavaScript as execute, mas ainda mantém o código disponível para referência ou reativação posterior.

##### Exemplo Simples:
```javascript
// Este código calcula o dobro de um número
// let numero = 5;
// let dobro = numero * 2;
// console.log(dobro);
```
Aqui, todo o bloco de código foi comentado. Isso desativa temporariamente a execução, mas o código ainda está presente e pode ser restaurado facilmente removendo os comentários.

##### Exemplo Prático:
Imagine que você esteja testando uma nova funcionalidade, mas não quer excluir o código antigo. Você pode comentar temporariamente o código original enquanto desenvolve a nova lógica.

```javascript
// Versão antiga - Calcula a média de dois números
// let numero1 = 10;
// let numero2 = 20;
// let media = (numero1 + numero2) / 2;
// console.log(media);

// Nova abordagem - Calcula a média de três números
let numero1 = 10;
let numero2 = 20;
let numero3 = 30;
let media = (numero1 + numero2 + numero3) / 3;
console.log(media);
```
Neste exemplo, o código antigo é desativado, permitindo que a nova abordagem seja testada sem remover o código anterior.

- **Considerações:**
  - **Evite incluir código desativado na versão final do projeto.** Isso pode confundir outros desenvolvedores e aumentar a complexidade do código sem necessidade.
  - Mantenha o código desativado apenas durante o desenvolvimento ativo. Após decidir pela implementação final, remova o código desativado para manter o código base limpo e organizado.

---

### 4. Documentação

#### **JSDoc**

**JSDoc** é uma ferramenta popular para a criação de documentação automatizada para código JavaScript. Ele permite que você adicione anotações diretamente no código, que podem ser processadas para gerar documentação formal. Isso é particularmente útil para projetos maiores, onde a clareza sobre o funcionamento das funções e seus parâmetros é crucial.

- **Por que usar JSDoc?**
  JSDoc ajuda a manter a documentação atualizada e integrada com o código. Ao adicionar anotações diretamente no código, você garante que a documentação reflete exatamente o que o código faz, minimizando a possibilidade de desatualização.

- **Estrutura básica do JSDoc:**
  As anotações do JSDoc geralmente ficam no início das funções, métodos ou classes e são envolvidas em blocos de comentários multilinha com uma sintaxe específica.

##### Exemplo Simples:
```javascript
/**
 * Calcula a soma de dois números.
 * @param {number} a - O primeiro número.
 * @param {number} b - O segundo número.
 * @returns {number} - A soma dos dois números.
 */
function somar(a, b) {
  return a + b;
}
```
Neste exemplo, as anotações do JSDoc explicam o que a função faz, os parâmetros que ela aceita e o valor que ela retorna. Isso não apenas documenta a função para outros desenvolvedores, mas também pode ser usado por ferramentas para gerar documentação formal.

##### Detalhando as tags JSDoc:
- **@param**: Descreve os parâmetros da função. Inclui o tipo de dado (como `{number}` ou `{string}`) e uma breve descrição do parâmetro.
- **@returns**: Indica o tipo e a descrição do valor que a função retorna.

##### Exemplo com Tags Comuns:
```javascript
/**
 * Retorna uma saudação personalizada.
 * @param {string} nome - O nome da pessoa a ser saudada.
 * @param {string} [mensagem='Olá'] - A mensagem de saudação (opcional).
 * @returns {string} - A saudação completa.
 * @example
 * // Exemplo de uso:
 * console.log(saudacao('João')); // Saída: Olá, João!
 */
function saudacao(nome, mensagem = 'Olá') {
  return `${mensagem}, ${nome}!`;
}
```
Neste exemplo, usamos algumas tags importantes:
- **@param** descreve os parâmetros da função, incluindo um valor padrão (`mensagem = 'Olá'`).
- **@returns** explica o que a função retorna, que neste caso é uma string de saudação.
- **@example** mostra como a função pode ser usada na prática.

##### Mais tags úteis do JSDoc:
- **@throws**: Indica que a função pode lançar uma exceção.
- **@deprecated**: Marca uma função como obsoleta, sugerindo que ela não deve mais ser usada.
- **@see**: Adiciona uma referência a outra função ou documentação relacionada.

- **Exemplo utilizando @throws e @deprecated:**
```javascript
/**
 * Divide dois números.
 * @param {number} divisor - O número pelo qual o valor será dividido.
 * @throws {Error} - Lança um erro se o divisor for zero.
 * @returns {number} - O resultado da divisão.
 * @deprecated - Use a função dividirSeguro em vez desta.
 */
function dividir(numerador, divisor) {
  if (divisor === 0) {
    throw new Error("Divisão por zero não é permitida");
  }
  return numerador / divisor;
}
```
Este exemplo demonstra como documentar uma função que pode lançar uma exceção e avisa que a função está obsoleta.

---

### 5. Boas Práticas

#### **Clareza e Concisão**
Escrever comentários claros e concisos é essencial para garantir que eles realmente ajudem na compreensão do código e não se tornem um obstáculo. Comentários bem escritos melhoram a legibilidade do código e facilitam a manutenção.

- **Principais Diretrizes:**
  - **Seja Claro:** Certifique-se de que os comentários são fáceis de entender. Use uma linguagem simples e evite jargões técnicos desnecessários.
  - **Seja Conciso:** Evite comentários longos e redundantes. Comente apenas o que é necessário para entender o propósito do código.
  - **Atualize Comentários:** Mantenha os comentários atualizados conforme o código muda. Comentários desatualizados podem ser mais prejudiciais do que úteis.

##### Exemplo Simples:
```javascript
// Calcula o quadrado de um número
function quadrado(x) {
  return x * x;
}
```
O comentário é direto e explica claramente o que a função faz.

##### Exemplo de Comentário Redundante:
```javascript
// A variável 'soma' armazena o resultado da soma dos números
let soma = 5 + 3; // Aqui, 'soma' é igual a 8
```
Aqui, o comentário é redundante porque o próprio código já deixa claro o que está acontecendo. Comentários como esse não acrescentam valor e devem ser evitados.

##### Exemplo de Comentário Útil:
```javascript
// Verifica se o número é par
function ehPar(numero) {
  return numero % 2 === 0; // Retorna verdadeiro se o número for divisível por 2
}
```
Neste exemplo, o comentário explica a condição lógica usada para determinar se o número é par, fornecendo uma visão adicional sobre o funcionamento da função.

#### **Evitar Comentários Redundantes**
Comentários devem complementar o código, não repetir o que o código já expressa claramente. Comentários redundantes podem poluir o código e dificultar a leitura.

##### Exemplo de Código com Comentários Redundantes:
```javascript
let idade = 30; // A variável 'idade' contém a idade da pessoa
```
Neste exemplo, o comentário é desnecessário porque o nome da variável já é autoexplicativo.

#### **Exemplo de Comentário Eficaz:**
```javascript
// Calcula o total de vendas aplicando o desconto
function calcularTotal(vendas, desconto) {
  let total = 0;
  for (let venda of vendas) {
    total += venda.preco - (venda.preco * desconto);
  }
  return total;
}
```
Aqui, o comentário fornece contexto sobre o propósito da função, esclarecendo que o cálculo envolve a aplicação de um desconto.

Claro! Vamos adicionar exemplos na seção de conclusão para ilustrar os principais pontos discutidos sobre **Comentários** em JavaScript.

---

### Conclusão

Comentários são uma parte vital da programação em JavaScript, pois ajudam a tornar o código mais compreensível e manutenível. Eles servem como uma forma de comunicação entre desenvolvedores e são essenciais para garantir que o código possa ser entendido e modificado facilmente por outros membros da equipe ou até mesmo pelo próprio autor em momentos futuros.

#### **Resumo dos Principais Pontos:**

1. **Importância dos Comentários:**
   Comentários ajudam a explicar o propósito e a lógica por trás do código, facilitando a colaboração e a manutenção.

   - **Exemplo de Comentário Explicativo:**
     ```javascript
     // Calcula o valor final do pedido com desconto aplicado
     function calcularValorFinal(preco, desconto) {
       return preco - (preco * desconto);
     }
     ```
     Neste exemplo, o comentário explica o objetivo da função, ajudando a entender rapidamente o que o código faz.

2. **Tipos de Comentários:**
   - **Comentários Inline:** Usados para explicar linhas específicas de código.
     - **Exemplo de Comentário Inline:**
       ```javascript
       let preco = 100; // Preço original do produto
       let desconto = 0.2; // Desconto de 20%
       ```
       O comentário explica o propósito das variáveis `preco` e `desconto`, fornecendo contexto adicional.

   - **Comentários Multilinha:** Usados para descrever blocos maiores de código ou fornecer descrições mais detalhadas.
     - **Exemplo de Comentário Multilinha:**
       ```javascript
       /*
         Esta função verifica se um número é positivo, negativo ou zero.
         - Retorna "positivo" se o número for maior que zero.
         - Retorna "negativo" se o número for menor que zero.
         - Retorna "zero" se o número for igual a zero.
       */
       function verificarNumero(num) {
         if (num > 0) return "positivo";
         if (num < 0) return "negativo";
         return "zero";
       }
       ```
       O comentário multilinha fornece uma descrição detalhada do que a função faz e como ela se comporta em diferentes casos.

3. **Desativação Temporária de Código:**
   Comentar código temporariamente permite que você teste ou experimente novas funcionalidades sem remover o código original.

   - **Exemplo de Desativação Temporária:**
     ```javascript
     // Código original para calcular a área do quadrado
     // let lado = 5;
     // let area = lado * lado;
     // console.log(area);

     // Novo código para calcular a área do círculo
     let raio = 7;
     let areaCirculo = Math.PI * raio * raio;
     console.log(areaCirculo);
     ```
     O código antigo está comentado, permitindo a experimentação com uma nova abordagem para o cálculo da área.

4. **Documentação com JSDoc:**
   JSDoc é uma ferramenta que gera documentação automatizada a partir de anotações no código, descrevendo funções, parâmetros e retornos.

   - **Exemplo de JSDoc:**
     ```javascript
     /**
      * Converte uma temperatura de Celsius para Fahrenheit.
      * @param {number} celsius - A temperatura em graus Celsius.
      * @returns {number} - A temperatura convertida em graus Fahrenheit.
      * @example
      * // Converte 25 graus Celsius para Fahrenheit
      * console.log(converterParaFahrenheit(25)); // Saída: 77
      */
     function converterParaFahrenheit(celsius) {
       return (celsius * 9/5) + 32;
     }
     ```
     O exemplo utiliza JSDoc para documentar a função, explicando o que ela faz e fornecendo um exemplo de uso.

5. **Boas Práticas:**
   Comentários devem ser claros, objetivos e relevantes, evitando redundâncias e mantendo o código limpo.

   - **Exemplo de Boa Prática:**
     ```javascript
     // Função para verificar se um número é par
     function ehPar(numero) {
       return numero % 2 === 0; // Retorna verdadeiro se o número for divisível por 2
     }
     ```
     O comentário explica a lógica usada na função, sem ser redundante ou desnecessário.

#### **Considerações Finais:**

Implementar boas práticas de comentários é essencial para a criação de código que não só funcione corretamente, mas que também seja fácil de entender e manter. Comentários eficazes ajudam a garantir que o código possa ser facilmente compreendido por outros desenvolvedores e por você mesmo no futuro. Ao seguir as diretrizes e exemplos fornecidos nesta seção, você pode melhorar significativamente a qualidade e a legibilidade do seu código JavaScript.

A documentação e os comentários bem escritos são ferramentas poderosas que contribuem para o sucesso de projetos de programação e facilitam a colaboração e a evolução contínua do software.