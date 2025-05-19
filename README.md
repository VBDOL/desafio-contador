# Desafio Controle de Fluxo

## 📌 Descrição
Este projeto implementa um **contador numérico** baseado nos parâmetros inseridos pelo usuário via terminal. O objetivo é exercitar conceitos de **controle de fluxo** em Java, utilizando estruturas condicionais, exceções personalizadas e loops.

## 🛠 Funcionalidades
- O usuário informa **dois números inteiros** no terminal.
- O sistema verifica se o primeiro número **é menor** que o segundo.
- Se for válido, o sistema exibe números incrementados até atingir o limite.
- Caso contrário, é lançada a **exceção personalizada** `ParametrosInvalidosException`.

## 📜 Regras de Negócio
1. Se o **primeiro número** for maior que o **segundo número**, a exceção `ParametrosInvalidosException` é acionada.
2. Se os números forem válidos, o programa executa um **loop `for`**, imprimindo os números na tela.

## 📌 Estrutura do Projeto
### **Contador.java** (Classe Principal)
Esta classe é responsável por receber os valores do usuário, chamar o método de contagem e tratar possíveis exceções.

### **Método `contar(int parametroUm, int parametroDois)`**
- Verifica se `parametroUm` é **maior** que `parametroDois`. Se for, lança a exceção `ParametrosInvalidosException`.
- Calcula a quantidade de interações (`contagem = parametroDois - parametroUm`).
- Executa um loop `for` para imprimir os números.

### **ParametrosInvalidosException.java**
- Classe de exceção personalizada.
- Lançada quando `parametroUm` é maior que `parametroDois`.

## 💻 Exemplo de Execução
**Entrada do usuário no terminal:**

Digite o primeiro parâmetro 12 Digite o segundo parâmetro 30

**Saída esperada no console:**
Imprimindo o número 1 Imprimindo o número 2 Imprimindo o número 3 ... Imprimindo o número 18

Se a entrada for inválida:
Digite o primeiro parâmetro 30 Digite o segundo parâmetro 12

Saída:
O segundo parâmetro deve ser maior que o primeiro

## 🚀 Como Executar
1. **Clone** o repositório.
2. Compile o projeto: `javac Contador.java`
3. Execute o código: `java Contador`

### 📝 Contribuições
Fique à vontade para aprimorar o código ou sugerir melhorias! 😃

---
