Projeto: Eccomerce Online

Primeira Funcionalidade: Compra.

Regras de Negócio:

* O usuário deve estar logado para realizar uma compra.
* O produto deve estar disponível em estoque.
* O carrinho não pode estar vazio.
* O valor total deve ser calculado corretamente (produtos + frete).

Casos de Teste:

Caso 1 – Compra realizada com sucesso (Positivo).

* Entrada: Usuário logado, produto disponível, carrinho com itens.
* Resultado esperado: Compra finalizada com sucesso.
* Tipo: E2E.

Caso 2 – Compra com carrinho vazio (Negativo).

* Entrada: Usuário logado, carrinho sem produtos.
* Resultado esperado: Sistema impede a compra e exibe mensagem de erro.
* Tipo: Unitário.

Segunda Funcionalidade: Pagamento.

Regras de Negócio:

- O pagamento deve ser aprovado para concluir o pedido.
* Métodos de pagamento válidos (cartão, PIX, boleto).
* Dados do pagamento devem ser preenchidos corretamente.
* O valor cobrado deve ser igual ao valor da compra.

Casos de Teste:

Caso 3 – Pagamento aprovado (Positivo).

* Entrada: Dados válidos de pagamento.
* Resultado esperado: Pagamento aprovado e pedido confirmado.
* Tipo: Integração.

Caso 4 – Pagamento recusado (Negativo).

* Entrada: Cartão inválido ou sem saldo.
* Resultado esperado: Pagamento recusado e mensagem de erro exibida.
* Tipo: Integração.

Terceira Funcionalidade: Login.

Regras de Negócio:

* O usuário deve informar e-mail e senha válidos.
* O sistema deve validar os dados com o banco.
* O acesso só é permitido com credenciais corretas.
* Após login, o usuário deve ser redirecionado para a área logada.

Casos de Teste:

Caso 5 – Login com sucesso (Positivo).

* Entrada: E-mail e senha corretos.
* Resultado esperado: Usuário autenticado e redirecionado.
* Tipo: Unitário.

Caso 6 – Login com senha incorreta (Negativo).

* Entrada: E-mail correto e senha incorreta.
* Resultado esperado: Acesso negado e mensagem de erro.
* Tipo: Unitário.
