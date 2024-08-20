### Prototypes

#### 1. Introdução aos Prototypes
   - **O que é o Prototype?**
     - Explicação da herança baseada em protótipos no JavaScript.
     - Como todos os objetos em JavaScript possuem um prototype.
   - **O Modelo de Herança Prototípica**
     - Comparação entre herança prototípica e herança baseada em classes em outras linguagens.
     - Explicação sobre a relação entre instâncias e seus prototypes.

#### 2. A Cadeia de Prototypes
   - **Prototype Chain**
     - Como funciona a cadeia de prototypes (Prototype Chain).
     - Como JavaScript busca propriedades e métodos na cadeia de prototypes.
   - **Herança de Propriedades e Métodos**
     - Herança de propriedades de prototypes através da cadeia.
     - Como objetos podem acessar propriedades que não estão diretamente neles, mas nos seus prototypes.

#### 3. Manipulação de Prototypes
   - **Propriedade `__proto__`**
     - Explicação sobre a propriedade `__proto__` e sua função na ligação entre um objeto e seu prototype.
   - **Método `Object.getPrototypeOf()`**
     - Como obter o prototype de um objeto.
   - **Método `Object.setPrototypeOf()`**
     - Como alterar o prototype de um objeto e suas implicações.
   - **Propriedade `prototype` nas Funções**
     - Como a propriedade `prototype` em funções construtoras afeta os objetos instanciados por elas.

#### 4. Funções Construtoras e Prototypes
   - **Relação entre Funções Construtoras e Prototypes**
     - Como funções construtoras criam objetos que possuem o mesmo prototype.
   - **Adição de Métodos ao Prototype**
     - Como adicionar métodos diretamente ao prototype para serem compartilhados entre todas as instâncias de um objeto.
     - Exemplo prático: criação de métodos usando a propriedade `prototype`.

#### 5. `Object.create()` e Prototypes
   - **Criação de Objetos com Prototypes Específicos**
     - Uso do método `Object.create()` para criar objetos com um prototype especificado.
   - **Herança Simulada com `Object.create()`**
     - Como `Object.create()` pode ser usado para criar padrões de herança personalizados.

#### 6. Boas Práticas e Considerações
   - **Evitar Manipulação Direta de `__proto__`**
     - Explicação dos riscos de manipulação direta de `__proto__` e melhores alternativas.
   - **Uso Estratégico de Prototypes para Performance**
     - Como o uso correto de prototypes pode melhorar a performance e evitar duplicação de código.
   - **Prototypes vs Classes Modernas**
     - Comparação entre a herança baseada em protótipos e a introdução de classes no ES6.