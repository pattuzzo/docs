### Tipos de Dados

#### 1. Tipos Primitivos
   - **Undefined**
     - Definição e Comportamento
     - Diferença entre Undefined e Null
   - **Null**
     - Definição e Propósito
     - Uso Prático e Armadilhas Comuns
   - **Boolean**
     - Definição e Uso de Verdadeiro/Falso
     - Coerção de Tipos em Operações Booleanas
   - **Number**
     - Números Inteiros e de Ponto Flutuante
     - Precisão e Limitações (Infinity, NaN)
   - **BigInt**
     - Definição e Manipulação de Números Grandes
     - Diferenças entre BigInt e Number
   - **String**
     - Definição e Operações Básicas com Strings
     - Imutabilidade e Métodos Comuns
   - **Symbol**
     - Definição e Uso para Identificadores Únicos
     - Aplicações Avançadas de Symbols (Ex: Propriedades Privadas)

#### 2. Tipos Compostos
   - **Array**
     - Definição e Comportamento de Arrays
     - Métodos e Operações Comuns em Arrays
     - **Array Multidimensional**
       - Arrays Aninhados e Acesso a Elementos
   - **Object**
     - Definição e Estrutura de Objetos
     - Criação e Manipulação de Propriedades
     - **Object.prototype**
       - Métodos Comuns (`Object.keys()`, `Object.values()`, `Object.entries()`, `Object.assign()`)

#### 3. Estruturas de Dados
   - **Estruturas de Coleção**
     - **Set**
       - Definição e Manipulação de Conjuntos Únicos
     - **WeakSet**
       - Diferenças entre Set e WeakSet
       - Uso para Coleções de Objetos
     - **Map**
       - Definição e Manipulação de Mapas Chave/Valor
     - **WeakMap**
       - Diferenças entre Map e WeakMap
       - Uso em Casos de Chaves Temporárias
   - **Iterável**
     - Definição e Comportamento dos Iteráveis
     - Uso de `for...of`, `Symbol.iterator` e Iteradores Personalizados

#### 4. Operadores de Tipos
   - **Operador `typeof`**
     - Comportamento e Casos Especiais (ex: `typeof null`)
     - Exemplos Práticos e Limitações
   - **Operador `instanceof`**
     - Verificação de Instância de Objetos
     - Comparação com `typeof` e Limitações
     - Exemplo com Cadeias de Herança

#### 5. Conversão de Tipos
   - **Coerção Implícita e Explícita**
     - Coerção Automática pelo JavaScript (Exemplos Comuns)
     - Diferença entre Conversão Implícita e Explícita
   - **Conversão Explícita**
     - **Boolean**
       - Conversão de Tipos Diferentes para Booleano
     - **Number**
       - Conversão de Strings e Outros Tipos para Número
       - Limitações e Armadilhas (ex: `parseInt`, `parseFloat`)
     - **BigInt**
       - Conversão Explícita para BigInt e Limitações
     - **String**
       - Conversão de Tipos para String (ex: `.toString()`, `String()`)
     - **Array**
       - Conversão de Iteráveis e Objetos em Arrays
       - Métodos de Conversão (ex: `Array.from`, Spread Operator)
   - **Coerção de Tipos em Comparações**
     - Diferenças entre `==` e `===`
     - Exemplos de Coerção Implícita (ex: `'' == 0`, `null == undefined`)

#### 6. Tipos de Dados Dinâmicos
   - **Dynamic Typing (Tipagem Dinâmica)**
     - Conceito de Tipagem Dinâmica
     - Vantagens e Desvantagens
     - Exemplos Práticos e Desafios
   - **Duck Typing**
     - Conceito e Definição
     - Comparação com Verificação Explícita de Tipos
     - Exemplos de Implementação