# 💰 Soma Filtrada de Produtos com Predicate (Java)

Este projeto demonstra como usar a interface funcional `Predicate` com expressões lambda em Java para calcular a soma dos preços de produtos 
que atendem a um critério definido — neste caso, produtos cujo nome começa com a letra **"T"**.

---

## 🚀 Objetivo

- Calcular a soma dos preços de produtos filtrados.
- Aplicar programação funcional com a interface `Predicate<T>`.
- Praticar boas práticas de organização, com separação da lógica em uma classe de serviço.

---

## 🧩 Estrutura do Projeto

src/
├── app/
│ └── Program.java // Classe principal
├── model/
│ ├── entities/
│ │ └── Product.java // Representa um produto (nome + preço)
│ └── services/
│ └── ProductService.java // Contém o método filteredSum

---

## 🔧 Como funciona

1. Cria-se uma lista de produtos com nome e preço.
2. Usa-se o método `filteredSum`, da classe `ProductService`, passando:
   - A lista de produtos.
   - Um predicado (`p -> p.getName().charAt(0) == 'T'`) que seleciona apenas produtos cujo nome começa com "T".
3. O método percorre a lista, soma os preços dos produtos que atendem ao critério e retorna o total.
4. O resultado é exibido no console.

---

### 🔍 Código-chave

```java
double sum = ps.filteredSum(list, p -> p.getName().charAt(0) == 'T');

📌 Exemplo de Saída

Sum = 1250.50

📚 Conceitos Utilizados

    Java 8+

    Interface funcional Predicate<T>

    Expressões lambda

    API de coleções (List)

    Encapsulamento de lógica com classe de serviço (ProductService)

    Separação de responsabilidades

▶️ Como Executar
Requisitos:

    JDK 8 ou superior

    IDE Java ou terminal

Via terminal:

javac app/Program.java
java app.Program

👩‍💻 Autora

Daniela Alineri 👩‍💻
