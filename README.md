# Sistema Bancario simples- Desafio DIO

Este é um simples sistema bancário implementado em Python como desafio de projeto para o bootcamp Python BackEnd Vivo na plataforma DIO. Ele permite que os usuários realizem operações básicas como depósito, saque e visualização do extrato.

## Funcionalidades
--------------------------------------------------------------------------------------------------

O sistema oferece as seguintes funcionalidades:

- **Depositar**: Permite ao usuário depositar um valor em sua conta.
- **Sacar**: Permite ao usuário sacar um valor de sua conta. O valor do saque não pode exceder o saldo atual da conta nem o limite de saque definido.
- **Extrato**: Permite ao usuário visualizar todas as transações realizadas.
- **Sair**: Permite ao usuário sair do sistema.

## Explicação do Código
---------------------------------------------------------------------------------------------------

O código é um sistema bancário simples implementado em Python. Aqui está uma explicação passo a passo:

1. **Variáveis Iniciais**: No início do código, definimos algumas variáveis. `saldo` é o saldo inicial da conta do usuário, `limite` é o limite de saque, `extrato` é uma string vazia que armazenará o histórico de transações, `numero_saques` é o número de saques realizados e `LIMITE_SAQUES` é o número máximo de saques permitidos.

2. **Menu de Opções**: Em seguida, temos um menu de opções que é exibido para o usuário. O usuário pode escolher entre depositar dinheiro (`d`), sacar dinheiro (`s`), ver o extrato (`e`) ou sair do sistema (`q`).

3. **Loop Principal**: O código então entra em um loop infinito, onde solicita ao usuário que escolha uma opção do menu.

4. **Depósito**: Se o usuário escolher a opção de depósito (`d`), o código solicitará ao usuário que informe o valor do depósito. Se o valor for maior que 0, o valor será adicionado ao saldo e uma entrada de depósito será adicionada ao extrato.

5. **Saque**: Se o usuário escolher a opção de saque (`s`), o código solicitará ao usuário que informe o valor do saque. O código então verifica se o valor do saque excede o saldo, o limite de saque ou o número máximo de saques. Se o valor do saque for válido, ele será subtraído do saldo e uma entrada de saque será adicionada ao extrato.

6. **Extrato**: Se o usuário escolher a opção de extrato (`e`), o código imprimirá todas as transações realizadas e o saldo atual.

7. **Sair**: Se o usuário escolher a opção de sair (`q`), o código quebrará o loop e o programa será encerrado.

8. **Opção Inválida**: Se o usuário escolher uma opção que não seja `d`, `s`, `e` ou `q`, o código imprimirá uma mensagem informando que a operação é inválida e solicitará que o usuário selecione novamente a operação desejada.
