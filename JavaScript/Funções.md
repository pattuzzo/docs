### Funções

#### **1. Introdução às Funções**
- **O que são Funções?**
  - Definição e propósito das funções em JavaScript.
  - Como funções permitem a reutilização de código e abstração.

#### **2. Tipos de Funções**
- **Função Literal**
  - Declaração de funções usando a forma literal, com exemplo simples.
  
- **Expressão de Função**
  - Definição e uso de funções como expressões, incluindo exemplos básicos.
  
- **Função Dinâmica**
  - Discussão sobre funções criadas dinamicamente, como usando o construtor `Function`.

#### **3. Declaração de Funções**
- **Função Nomeada**
  - Como declarar e usar funções nomeadas, incluindo exemplos e boas práticas.

- **Expressões de Função**
  - **Função Nomeada**
    - Diferença entre funções nomeadas em expressões e funções nomeadas declaradas.
  - **Função Anônima**
    - Declaração e uso de funções anônimas, como em callbacks e IIFE.
  - **Função de Seta (Arrow Function)**
    - Sintaxe e vantagens das funções de seta, incluindo exemplos e diferenças com funções tradicionais.
  - **Função Autoinvocada (IIFE)**
    - O que são IIFE (Immediately Invoked Function Expressions) e por que usá-las.

#### **4. Parâmetros e Argumentos**
- **Parâmetros**
  - **Parâmetros Opcionais**
    - Como definir e usar parâmetros opcionais.
  - **Parâmetro Rest**
    - Uso do parâmetro rest (`...args`) para capturar múltiplos argumentos em uma função.
  - **Desestruturação de Parâmetros**
    - Como utilizar desestruturação de objetos e arrays nos parâmetros de função.

- **Argumentos**
  - **Passagem de Parâmetros**
    - Como passar argumentos para funções e os tipos de dados que podem ser passados.
  - **Operador Spread**
    - Uso do operador spread (`...`) para expandir argumentos de uma função.

#### **5. Retorno da Função**
- **Valor de Retorno**
  - Como uma função retorna valores e o que acontece se não houver uma declaração `return`.

#### **6. Escopo de Função**
- **Variáveis**
  - Escopo local e global dentro de funções e como isso afeta o acesso às variáveis.

- **Içamento (Hoisting)**
  - O conceito de içamento de funções e variáveis em JavaScript.
  - Como o içamento afeta a declaração e chamada de funções, e as diferenças entre içamento de declarações e expressões de função.
  
- **Closure**
  - Definição de closures e exemplos práticos de como funções podem "lembrar" do ambiente em que foram criadas.

#### **7. Contexto `this` em Funções**
- **Método `call`**
  - Uso do método `call` para invocar funções com um contexto específico.
  
- **Método `apply`**
  - Uso do método `apply` para passar argumentos como um array para funções.
  
- **Método `bind`**
  - Como o método `bind` cria uma nova função com um contexto específico e argumentos fixos.

#### **8. Pilha de Chamadas**
- **O que é a Pilha de Chamadas?**
  - Explicação sobre a pilha de chamadas (call stack) e como ela gerencia a execução das funções.

#### **9. Objeto de Função**
- **Propriedades de Função**
  - **name**
    - Como acessar o nome da função usando a propriedade `name`.
  - **length**
    - Como a propriedade `length` representa o número de parâmetros formais da função.

- **Objeto de Argumentos**
  - **`arguments.length`**
    - Uso da propriedade `arguments.length` para determinar o número de argumentos passados a uma função.

#### **10. Funcionalidades Avançadas**
- **Recursividade**
  - O conceito de recursividade e exemplos de funções recursivas.
  
- **Construtor de Objetos**
  - Uso de funções construtoras para criar objetos e como isso se relaciona com a programação orientada a objetos.

- **Funções de Ordem Superior**
  - **Callbacks**
    - Uso de funções como argumentos para outras funções.
  - **Currying**
    - O que é currying e como ele permite a criação de funções com múltiplos parâmetros.
  
- **Funções Geradoras**
  - Introdução às funções geradoras e o uso de `yield` para gerar uma sequência de valores.

- **Funções Assíncronas**
  - Como funções assíncronas (`async/await`) permitem a execução de código assíncrono mais legível.

- **Decoradores**
  - O que são decoradores e como eles podem ser usados para modificar o comportamento de funções e classes (notar que a proposta de decoradores ainda está em estágio de proposta na especificação ECMAScript).