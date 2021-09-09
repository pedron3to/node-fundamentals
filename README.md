## FinAPI - Financeira

### Requisites

[] Be Possible to create an account;
_ Method - POST
_ Resource - account

[x] Deve ser possível buscar o extrato bancário do cliente
_ Qual o cliente? (Utilizar um middleware)
[x] Deve ser possível realizar um depósito
Condição para um depósito:
_ Data de criação;
_ Descrição do depósito
_ Quantidade \* Tipo (credito)
[x] Deve ser possível realizar um saque
Condição para um saque:
_ Data de criação;
_ Quantidade: Tipo (credito)
[x] Deve ser possível buscar o extrato bancário do cliente por data
condição para o saque:

- verificar se existe o cliente (middleware)
- receber um data(query params)
- filtrar extrato do cliente por data
  [x] Deve ser possível atualizar dados da conta do cliente
  - utilizar o método PUT

[x] Deve ser possível obter dados da conta do cliente

- utilizar o método GET
  [ x] Deve ser possível deletar uma conta
  * utilizar o splice pra tirar de dentro do array

  Deve ser possivel retornar o saldo.

## Regras de Negócio

[X] Não deve ser possível cadastrar um conta com CPF já existente

[x] Não deve ser possível fazer depósito em uma conta não existente
[x] Não deve ser possível buscar extrato em uma conta não existente
[x] Não deve ser possível fazer saque em uma conta não existente
[x] Não deve ser possível fazer saque quando o saldo for insuficiente
_ Precisa receber a quantia para o saque;
_ precisa receber o cliente;
_ precisa fazer o saldo (middleware);
_ utilizar o reduce()
_ verificar se o saldo < que a quantia para o saque
_ Condição para um depósito:
_ Data de criação;
_ Quantidade \* Tipo (debito)

[x] Não deve ser possível excluir uma conta não existente
