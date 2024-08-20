### Programação Assíncrona

#### **1. Conceitos Básicos**
- **Execução Síncrona vs Execução Assíncrona**
  - Definição e exemplos de execução síncrona.
  - Diferença entre tarefas síncronas e assíncronas.
  - Exemplos práticos para ilustrar a diferença e a importância da programação assíncrona em ambientes como o navegador e o Node.js.

- **Pilha de Chamadas (Call Stack)**
  - Explicação detalhada sobre a pilha de chamadas e seu papel na execução do código.
  - Exemplos visuais para ajudar na compreensão da pilha de chamadas em cenários síncronos e assíncronos.

- **Event Loop**
  - O funcionamento do **Event Loop** e sua importância na execução assíncrona.
  - **Microtasks**: Discussão sobre a fila de microtarefas, incluindo `Promise.then()` e `MutationObserver`.
  - **Macrotasks**: Explicação sobre a fila de macrotarefas, incluindo exemplos com `setTimeout()`, `setInterval()` e I/O.

#### **2. Callbacks**
- **Callback Hell**
  - Explicação sobre o fenômeno do "Callback Hell" e por que ele é problemático.
  - Como lidar com o Callback Hell e introdução às Promises como solução.

- **Fila de Callbacks**
  - Como os callbacks são enfileirados e executados dentro do Event Loop.
  - Diferença entre callbacks de microtarefas e macrotarefas.

#### **3. Promises**
- **Introdução às Promises**
  - O que são Promises e como elas representam o eventual sucesso ou falha de uma operação assíncrona.
  - Comparação entre Promises e callbacks para mostrar suas vantagens.

- **Estados das Promises**
  - **Pendente**: Explicação sobre o estado inicial de uma Promise.
  - **Resolvido**: O que significa quando uma Promise é resolvida.
  - **Rejeitado**: O que significa quando uma Promise é rejeitada.

- **Métodos das Promises**
  - **then()**: Como encadear ações que dependem da resolução de uma Promise.
  - **catch()**: Tratamento de erros com Promises.
  - **finally()**: Executando código independente do resultado da Promise.

- **Promise API**
  - **Métodos de Estados**
    - **resolve()**: Forçar a resolução de uma Promise com sucesso.
    - **reject()**: Forçar a rejeição de uma Promise.
  - **Métodos de Competição**
    - **race()**: Retorna a primeira Promise a ser resolvida ou rejeitada.
    - **any()**: Retorna a primeira Promise resolvida, ignorando rejeições.
  - **Métodos de Agregação**
    - **all()**: Espera todas as Promises serem resolvidas ou rejeitadas.
    - **allSettled()**: Retorna após todas as Promises terem sido concluídas, independentemente do resultado.
  - **Promise.withResolvers()**
    - Explicação deste padrão útil para resolver e rejeitar Promises manualmente dentro de uma função personalizada.

- **Encadeamento de Promises**
  - Exemplo prático de como encadear Promises para construir fluxos assíncronos mais claros.
  - Importância do encadeamento no tratamento de operações dependentes.

- **Promisificação**
  - Explicação sobre a conversão de funções baseadas em callbacks para retornarem Promises.
  - Exemplos de código mostrando como a promisificação melhora a legibilidade.

#### **4. Async/Await**
- **Introdução ao Async/Await**
  - Como `async` e `await` facilitam a escrita de código assíncrono que parece síncrono.
  - Diferença de comportamento em comparação às Promises e seus benefícios.

- **Tratamento de Erros**
  - Como lidar com erros usando `try/catch` em funções `async`.
  - Vantagens de usar `async/await` no tratamento de erros em comparação com o uso de `catch()` em Promises.

#### **5. Temporizadores**
- **Tipos de Temporizadores**
  - **setTimeout**: Agendamento de funções após um atraso especificado.
  - **setInterval**: Execução repetitiva de funções em intervalos especificados.
  - Exemplos de casos práticos de uso, como animações e polling de dados.

- **Limpeza de Agendamento**
  - **clearTimeout()** e **clearInterval()**: Como e quando cancelar temporizadores para evitar comportamentos indesejados ou vazamentos de memória.

#### **6. Web Workers e Service Workers**
- **Web Workers**
  - Introdução ao conceito de Web Workers e como eles permitem a execução de código em threads separadas.
  - Quando usar Web Workers para melhorar a performance e evitar o bloqueio do Event Loop.
  - Exemplo básico de criação e comunicação com Web Workers.

- **Service Workers**
  - O que são Service Workers e seu papel em fornecer experiências offline e cache para aplicações web.
  - Como os Service Workers funcionam e são registrados.
  - Exemplos práticos de uso, como cache de recursos e interceptação de requisições de rede.