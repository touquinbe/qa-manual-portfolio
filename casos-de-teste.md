**ID: CT-001**
Título: Login válido
Pré-condição: Reconhecimento de usuário 
Passos:
**01** - Abrir o site
**02** - Inserir usuário válido
**03** - Inserir senha válida 
**04** - Clicar em login
Resultado esperado: Usuário é redirecionado para a página de produtos. 
**Status**: **Passou**

**ID: CT-002**
Título: Login inválido
Pré-condição: Reconhecimento de usuário 
Passos:
**01.** Abrir o site
**02.** Inserir usuário inválido
**03.** Inserir senha inválida 
**04.**  Clicar em login
Resultado esperado: O sistema exibe mensagem de erro informando falha na autenticação.
**Status**: **Passou**

**ID: CT-003**
Título: Adicionar produto no carrinho
Pré-condição: Usuário logado/Produto disponível 
Passos:
**01.** Selecionar o produto e adicionar ao carrinho
**02.** Acessar carrinho
Resultado esperado: O produto é exibido corretamente no carrinho.
**Status: Passou**

**ID: CT-004**
Título: Remover produto no carrinho
Pré-condição: Usuário logado/Produto dentro do carrinho
Passos:
**01.** Abrir carrinho
**02.** Clicar em remover do carrinho
Resultado esperado: Usuário consegue remover item do carrinho.
**Status: Passou**

**ID: CT-005**
Título: Finalizar compra
Pré-condição: Usuário logado/Produto dentro do carrinho
Passos:
**01.** Abrir carrinho
**02.** Clicar em Prosseguir
**03.** Adicionar informações de endereço e método de pagamento
**04.** Finalizar compra.
Resultado esperado: Solicitação realizada com sucesso.
**Status: Reprovou

[BUG] Tela em branco ao finalizar compra no fluxo de checkout
Ambiente:
- Navegador: - Chrome
             - Safari
- Sistema operacional: - IOS 
                       - Windows
- URL: [saucedemo.com](http://saucedemo.com/)
Passos para reproduzir:
1. Realizar login com usuário válido
2. Adicionar produto ao carrinho
3. Acessar carrinho
4. Clicar em "Prosseguir"
5. Preencher dados obrigatórios
6. Clicar em avançar

**Resultado esperado:**
Sistema deve concluir a compra e exibir confirmação ao usuário
**Resultado obtido:**
Sistema exibe página em branco sem retorno ao usuário
**Severidade:** Alta
**Prioridade:** Alta
