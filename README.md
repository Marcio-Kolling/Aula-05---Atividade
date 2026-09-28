Cada correção de erro está em uma branch individual. A última branch é a versão final com todas as correções. (Na branch do erro 6 há também um último ajuste no flexbox).

1 - Cascata: havia um '!important' na regra do 'h1', que dava prioridade desnecessária à declaração. Removi o '!important'.

2 - Especificidade: a regra '#cardapio .preco' era mais específica que '.promocao' e impedia o preço promocional de ficar vermelho. Ajustei a especificidade da regra da promoção.

3 - Box model: os cartões utilizavam 'width: 100%' junto com padding e borda, fazendo sua largura ultrapassar o espaço disponível. Usei 'box-sizing: border-box' e ajustei o dimensionamento com Flexbox (Correção adicional no erro 6).

4 - Contraste: o subtítulo utilizava uma cor muito clara sobre o fundo branco. Escureci a cor para melhorar a legibilidade.

5 - Foco: 'outline: none' removia a indicação visual de foco dos links do menu. Substituí por um estilo de foco visível com ':focus-visible'.

6 - Alinhamento: o menu era deslocado usando 'margin-left: 610px', um valor fixo que não se adapta à tela. Usei Flexbox no topo com 'justify-content: space-between'. Como adicional, foi corrigido o flexbox dos botões no canto superior direito da tela para ficarem na horizontal e não na vertical.
