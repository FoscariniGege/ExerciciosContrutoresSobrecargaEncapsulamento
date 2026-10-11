# ☕ Módulo: Introdução a Classes e Orientação a Objetos (POO) em Java

Este repositório documenta a consolidação da minha base em Programação Orientada a Objetos (POO) com Java. Esta pasta centraliza os primeiros **7 exercícios práticos** do curso, representando a transição crucial da programação estruturada/procedural para uma arquitetura limpa, modular e orientada a objetos, aplicando boas práticas de Código Limpo (*Clean Code*).

---

## 🚀 O que foi treinado e aplicado no módulo

- **Separação de Pacotes (`application`, `entities` e `util`)**: Isolamento claro entre o ponto de entrada da aplicação, regras de negócio das entidades e classes utilitárias.
- **Construtores e Sobrecarga (*Overloading*)**: Inicialização controlada dos objetos permitindo instanciar classes de formas diferentes conforme a presença ou ausência de dados opcionais.
- **Encapsulamento e Modificadores de Acesso (`private`)**: Proteção do estado interno dos objetos, expondo apenas os dados necessários por meio de *getters* e restringindo alterações indevidas via ausência de *setters*.
- **Atributos e Métodos de Instância**: Compreensão de moldes de classes e como cada objeto manipula seu próprio estado de forma isolada.
- **Membros Estáticos (`static`) e Constantes (`final`)**: Criação de rotinas utilitárias sem a necessidade de criar instâncias (`new`) e definição de valores imutáveis de classe.
- **Mutabilidade de Estado e Regras de Negócio**: Métodos dedicados para alterar atributos sob regras específicas (ex: acréscimo de depósitos, desconto de taxas em saques, reajustes percentuais).
- **Sobrescrita do método `toString()`**: Customização da representação textual dos objetos para manter a classe principal enxuta e legível.

---

## 💻 Os 7 Exercícios Resolvidos nesta Pasta

1. **Calculadora de Área de Triângulos (`Triangle`)**:
   - *Evolução Inicial*: Comparação prática da mesma lógica primeiro de forma procedural (variáveis soltas no `main`) e, em seguida, modularizada em uma classe dedicada aplicando a Fórmula de Heron.
2. **Controle de Estoque de Produtos (`Product`)**:
   - *Foco*: Gerenciamento de estado e fluxo de mercadorias. O sistema calcula o valor total em estoque, realiza entradas (`addProducts`) e saídas (`removeProducts`), exibindo o estado atualizado com o `toString()`.
3. **Cálculo de Medidas do Retângulo (`Rectangle`)**:
   - *Foco*: Encapsulamento de fórmulas geométricas. A classe calcula de forma independente a Área, o Perímetro e a Diagonal (utilizando o Teorema de Pitágoras com `Math.sqrt`).
4. **Gestão de Funcionários (`Employee`)**:
   - *Foco*: Mutabilidade e regras de negócio financeiras. O sistema calcula o salário líquido descontando impostos e aplica aumentos percentuais com impacto direto no salário bruto do colaborador.
5. **Sistema de Avaliação de Alunos (`Student`)**:
   - *Foco*: Lógica condicional e formatação dinâmica. A classe soma as notas dos trimestres, avalia a situação do aluno (aprovação/reprovação) e calcula quantos pontos faltaram para atingir a nota de corte em caso de reprovação.
6. **Conversor de Moeda com IOF (`ConversorDeDinheiro` / `CurrencyConverter`)**:
   - *Foco*: Membros estáticos e classes utilitárias. Centralização do cálculo de câmbio em uma classe utilitária estática, aplicando constante (`IOF = 0.06`) e método estático sem instanciação.
7. **Sistema de Conta Bancária (`ContaBancaria`)**:
   - *Foco*: Construtores, sobrecarga e encapsulamento rígido. O número da conta é imutável (`final` e sem setter), o saldo só é modificado via operações de depósito e saque (com desconto de tarifa fixa de R$ 5,00), e a abertura da conta suporta tanto abertura com depósito inicial opcional quanto com saldo zero através de sobrecarga de construtores.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas

- **Linguagem**: Java
- **Entrada e Saída**: `Scanner`, `Locale.US`, `System.out.printf` e `String.format` (formatação de casas decimais e quebras de linha com `%n`)
- **Bibliotecas Nativas**: `java.lang.Math`
- **Conceitos de POO e Boas Práticas**:
  - Encapsulamento (`private`, Getters e Setters controlados)
  - Construtores Padrão e Sobrecarga de Construtores
  - Métodos de Instância vs. Métodos Estáticos (`static`)
  - Constantes de Classe (`static final`)
  - Sobrescrita de Métodos (`@Override toString`)
  - Separação de Responsabilidades em Camadas/Pacotes (`application`, `entities`, `util`)

