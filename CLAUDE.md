# Ambimulty

## Working preferences
- Fale e escreva sempre em português com o usuário: mensagens, avisos de progresso, resumos, perguntas e descrições das versões salvas do tema. Os textos da loja (para o cliente) continuam em inglês britânico.
- Centralize tudo com precisão: ícone dentro de círculo ou pílula fica no centro exato; use SVG desenhado centrado (viewBox 24x24, forma em 12,12), nunca caracteres de texto como → ou +.
- Mantenha a mesma estrutura em toda a loja: uma margem lateral única, um ritmo fixo de espaços entre seções, títulos e cartões; nada encostando.
- Meça alinhamento e espaçamento (screenshot e medição) antes de entregar; não confie no olho.
- Verifique todas as páginas (home, produto, coleção, FAQ, políticas, rastreio, carrinho, busca, 404) antes de entregar; um erro corrigido numa página não pode continuar nas outras.
- Efeitos: micro-interações sutis e dentro da marca (verde-limão, verde-floresta, pílulas, títulos grandes), sempre respeitando "reduzir movimento".
- Versão nova do tema feita duplicando o tema ao vivo leva só o que está publicado: compare arquivo por arquivo com a versão salva e reaplique o que faltar antes de entregar (já trouxe de volta coisas removidas na v43 e na v48).
- Uma página, um produto: a página de cada produto fala só daquele produto (título, destaque, benefícios, faixa verde, números, passos, descrição). Nunca citar outro produto. O template padrão `templates/product.json` fica genérico, sem texto de produto nenhum; cada produto com conteúdo próprio ganha seu template `product.<handle>.json` e o produto aponta para ele. Ao adicionar produto novo, conferir a página dele no tema ao vivo antes de dizer que está pronto.
- Preço comparativo ("de £X por £Y"): o dono usa para mostrar desconto; a página mostra a economia calculada sozinha a partir do preço riscado. Lembrar que no Reino Unido o preço anterior precisa ser real.
- Nunca mostrar ao cliente a quantidade em estoque.
- Produto importado pelo DSers fica com estoque só no local do DSers, que não tem frete: ativar o produto também no local que tem frete, senão a página mostra "Unavailable".
- Produto com cores: cada cor tem a sua foto ligada à variante, para a galeria pular para a foto certa quando o cliente clica na cor. O nome da cor tem que bater com a foto (o Birdhaven veio do fornecedor com "Green" numa foto turquesa) e usar grafia britânica (Grey, Colour). Conferir abrindo a página com ?variant=<id> de cada cor.
