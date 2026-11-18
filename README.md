# 🌭 Dog dos AP

Site do Dog dos AP com cardápio interativo, carrinho de compras e envio de pedidos pelo WhatsApp. O projeto tem layout responsivo e uma animação de entrega que acompanha a rolagem da página.

🔗 **Acesse:** https://menezes0705.github.io/dogdosap/

## Funcionalidades

- Cardápio organizado por categorias.
- Busca por nome do produto ou ingrediente.
- Controles para adicionar e remover unidades.
- Carrinho salvo no navegador.
- Cálculo de subtotal, entrega e total.
- Validação do valor mínimo em produtos.
- Revisão do pedido com nome, endereço e observações.
- Envio do resumo para confirmação pelo WhatsApp.
- Indicador de loja aberta ou fechada, conforme o horário de Brasília.
- Animação ilustrativa de entrega.
- Layout adaptável a celulares, tablets e computadores.

> A animação não representa rastreamento em tempo real. O pedido precisa ser enviado no WhatsApp e confirmado pela equipe.

## Tecnologias

- HTML5
- CSS3
- JavaScript
- LocalStorage
- Google Fonts
- GitHub Pages

Não é necessário instalar dependências ou executar uma etapa de compilação.

## Como executar

1. Clone o repositório:

   git clone https://github.com/Menezes0705/dogdosap.git

2. Abra a pasta no Visual Studio Code.
3. Abra o arquivo `index.html` no navegador ou utilize a extensão Live Server.

As fontes externas e o acesso ao WhatsApp precisam de conexão com a internet.

## Organização do código

O projeto está disponível em duas versões:

### Arquivo único

O `index.html` completo reúne a estrutura, os estilos, os scripts e a imagem incorporada. Essa versão pode ser publicada diretamente na raiz do repositório.

### Arquivos separados

Para facilitar a manutenção, a versão organizada contém:

- `index.html`: estrutura da página.
- `style.css`: estilos, layout responsivo e animações.
- `data.js`: categorias, produtos, descrições e preços.
- `app.js`: busca, carrinho, horários e integração com WhatsApp.
- `assets/hotdog.jpg`: imagem ilustrativa.

Na versão com arquivos separados, mantenha os caminhos e envie todos os arquivos utilizados pela página.

## Personalização

### Cardápio

Edite a constante `CAT` para alterar categorias, nomes, descrições e preços dos produtos.

Na versão organizada, ela fica em `data.js`. Na versão de arquivo único, está dentro do `index.html`.

### WhatsApp

Procure por `5511956757740` e substitua pelo número desejado, usando código do país, DDD e número, sem espaços ou símbolos.

### Valores do pedido

Configuração atual:

- Entrega: R$ 5,00.
- Pedido mínimo em produtos: R$ 15,00.

Os cálculos utilizam centavos: `500` representa R$ 5,00 e `1500` representa R$ 15,00. Ao mudar esses valores, atualize também os textos correspondentes.

### Horários

- Terça a quinta: 18h às 22h50.
- Sexta e sábado: 18h às 23h50.
- Domingo e segunda: fechado.

O indicador utiliza o fuso `America/Sao_Paulo`. Alterações nos horários devem ser feitas tanto na lógica quanto nos textos exibidos.

## Publicação no GitHub Pages

Em **Settings → Pages**, configure:

- Source: Deploy from a branch.
- Branch: main.
- Pasta: /(root).

O arquivo de entrada deve ser o `index.html` da raiz.

Após cada commit na branch `main`, acompanhe a publicação na aba **Actions**.

## Funcionamento dos pedidos

1. O cliente seleciona os produtos.
2. O site calcula os valores.
3. O cliente revisa o carrinho e informa os dados de entrega.
4. O site abre o WhatsApp com o resumo preenchido.
5. O cliente envia a mensagem para a equipe confirmar o pedido.

O site não processa pagamentos nem confirma pedidos automaticamente.

## Armazenamento local

O carrinho é salvo no LocalStorage do navegador utilizado. Ele não é sincronizado entre dispositivos e pode ser apagado ao limpar os dados do navegador.

## Imagens e fontes

- Fotografia ilustrativa: Unsplash.
- Fontes: DM Sans e Barlow Condensed, disponibilizadas pelo Google Fonts.

As imagens ilustrativas não representam necessariamente a apresentação dos produtos vendidos.
