# Estudo sobre Componentes Controlados em React


## Controlled components vs. Uncontrolled components

### Introdução

Na maioria dos casos, o React recomenda o uso de componentes controlados para implementar formulários. Embora essa abordagem esteja alinhada com o modelo declarativo do React, os campos de formulário não controlados ainda são uma opção válida e têm seu mérito. Vamos analisar as diferenças entre as duas abordagens e quando você deve usar cada método.

### Uncontrolled Inputs (Entradas Não Controladas)

Entradas não controladas são como entradas de formulário HTML padrão:

- Elas mantêm seu próprio estado interno.
- Você recupera seus dados usando uma referência (ref) quando necessário (geralmente na submissão do formulário).
- São mais simples de usar em cenários básicos e requerem menos código.
- Podem ser uma boa escolha se você não precisa de validação em tempo real ou manipulação complexa dos dados de entrada.

### Controlled Inputs (Entradas Controladas)

Entradas controladas são gerenciadas pelo estado do React:

- O valor da entrada é controlado pelo estado do componente React.
- Mudanças na entrada atualizam o estado, que por sua vez atualiza o valor da entrada.
- Oferecem mais controle sobre o comportamento e os dados do formulário.
- São ideais para validação em tempo real, formatação de entrada e manipulações complexas.


## Comparação entre Componentes Controlados e Não Controlados

| Feature | Uncontrolled | Controlled |
|---------|--------------|------------|
| One-time value retrieval (e.g. on submit) | **Yes** | **Yes** |
| Validating on submit | **Yes** | **Yes** |
| Instant field validation | No | **Yes** |
| Conditionally disabling a submit button | No | **Yes** |
| Enforcing a specific input format | No | **Yes** |
| Several inputs for one piece of data | No | **Yes** |
| Dynamic inputs | No | **Yes** |
