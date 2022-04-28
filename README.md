# nivelamento_exercicio_black_friday

Objetivos: 
Uma Loja de Eletro precisa de uma página especial para Black Friday, onde os clientes geram descontos entre 40% e 90% para produtos surpresa (os produtos do array acima).

A aplicação deve iniciar com um botão central GERAR PROMOÇÃO e cada vez que o usuário clicar neste botão um valor entre 40 e 90 deve ser gerado aleatóriamente e usado para calcular o desconto em um produto aleatório da lista e apresentar somente o produto para o usuário.

1 - Crie o componente botão GERAR PROMOÇÃO e os states vinculados a ele.

Este botão gera um número random entre 1 e 6 e usa o método filter() para encontrar o produto com este id. 
Mostre apenas o produto com o mesmo id retornado pelo random e calcule o desconto entre 40% e 90%.

2 - Para apresentar as informações da promoção para o usuário, crie um state dentro do componente App e passe por props para o <ProductList/> para exibir cada produto dentro de um componente chamado <Product>.
Deve mostrar:

Nome do Produto
Preço original;
Porcentagem do desconto;
Valor do desconto;
Preço a ser pago,
Botão para adicionar ao seu carrinho.

3 - Crie uma função handleClick(productId) que adiciona o produto selecionado dentro de um state currentSale.

Dica: Passe a função handleClick por props até o componente <Product />.
Para adicionar itens no currentSale, a sua função handleClick terá que utilizar o método find(), para encontrar um item no array com o mesmo id recebido no parâmetro. 

4 - Crie uma segunda lista para mostrar os produtos que estão no array currentSale.

Mostre os produtos que estão no carrinho (currentSale). 
Esta lista também tem que mostrar:
Nome do Produto
Preço original;
Porcentagem do desconto;
Valor do desconto;
Preço a ser pago,
(sem o botão de adicionar). 

5 - Mostra o total do carrinho. Use o método reduce().
