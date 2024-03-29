<p align="center">
<img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E" />
<img src="https://img.shields.io/badge/Cypress-17202C?style=for-the-badge&logo=cypress&logoColor=white" />
</p>


- [Como executar](#como-executar)
- [Especificação do desafio](#especificação-do-desafio)
- [Plano de Testes](#plano-de-testes)
  - [Funcionalidades:](#funcionalidades)
  - [Cenários Principais:](#cenários-principais)
  - [Abordagem de Testes:](#abordagem-de-testes)
- [Atividade dos Testes](#atividade-dos-testes)
  - [Cadastro bem-sucedido](#cadastro-bem-sucedido)
  - [Login bem-sucedido](#login-bem-sucedido)
  - [Falha no Login](#falha-no-login)
  - [Processo de Compra](#processo-de-compra)

## Como executar

Siga estes passos para configurar e executar este projeto:

1. Garanta que você possui o Node.js e NPM (Node Package Manager) instalados em sua máquina
2. Clone este repositório em sua máquina
3. Instale as dependências do projeto:
   ```bash
   npm install
   ```
4. Abra a GUI do Cypress:
    ```bash
    npx cypress open
    ```

## Especificação
Para o site  [automationexercise](https://www.automationexercise.com/), realizar as seguintes atividades: 

- [x] Plano de testes e estratégia que cubra as funcionalidades de "Login", "Cadastro" e "Processo de Compra" no site 
- [x] Preparar um script automatizado com teste de regressão para o site citado, contendo as duas condições de testes abordadas: Cadastro e Login.  

## Plano de Testes

### Funcionalidades:
- Login 
- Cadastro
- Processo de compra no site.

### Cenários Principais:
- Registro bem-sucedido.
- Login bem-sucedido.
- Falhas de login.
- Processo de compra completo.

### Abordagem de Testes:
-  Automatizada

## Atividade dos Testes

### Cadastro bem-sucedido

  1. Clicar no botão de Login/Register na página inicial.
  2. Preencher os campos necessários no formulário de registro com os detalhes do usuário.
  3. Clicar no botão para criar a conta.
  4. Verificar se a mensagem de "Account Created!" é exibida.
  5. Continuar para a página inicial e verificar se o nome do usuário está correto.
  6. Clicar no botão para excluir a conta e verificar se a mensagem "Account Deleted!" é exibida.
### Login bem-sucedido
  1. Clicar no botão de Login/Register na página inicial.
  2. Preencher os campos de login com credenciais válidas
  3. Confirmar exibição do nome do usuário logado no Header da página
### Falha no Login
  1. Clicar no botão de Login/Register na página inicial.
  2. Preencher os campos de login com credenciais inexistentes
  3. A mensagem "Your email or password is incorrect!" deve ser exibida abaixo do formulário
### Processo de Compra 
  1. Fazer o login com um usuário registrado.
  2. Navegar para a página de produtos.
  3. Adicionar um produto ao carrinho.
  4. Ir para o carrinho.
  5. Verificar se o nome do produto adicionado está correto no carrinho.
  6. Avançar para o checkout. 
  7. Verificar se os detalhes de entrega coincidem com os do usuário.
  8. Preencher os detalhes do cartão de pagamento.
  9. Confirmar o pagamento e verificar se a mensagem "Order Placed!" é exibida.
