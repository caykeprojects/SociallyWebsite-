# SociallyWebsite

## Descrição do projeto

Este é um site simples de landing page para um aplicativo social. Ele usa HTML e CSS puros para apresentar uma seção hero com navegação, título, texto e imagem.

## Estrutura de arquivos

- `index.html` - arquivo principal da página.
- `style.css` - estilos aplicados ao layout e à aparência.
- `pictures/` - pasta com imagens usadas no site, como `logo.png`, `pic.png` e `back-image.png`.

## Como o HTML está organizado

- `<html lang="pt-BR">` define o idioma do conteúdo.
- `<head>` contém metadados e o link para o CSS.
- `<body>` contém a estrutura visual:
  - `.Hero` - container principal com fundo e altura mínima de tela cheia.
  - `<nav>` - barra de navegação com logo, itens de menu e botões.
  - `.content` - seção com título (`<h1>`), parágrafo (`<p>`) e botão de chamada para ação.
  - `<img class="recursos-img">` - imagem ilustrativa posicionada na parte inferior direita.

## Como o CSS funciona

- O reset global (`*`) remove margens e paddings padrões e define a fonte `Poppins`.
- `.Hero` define o fundo com imagem, tamanho e posicionamento, além de usar `position: relative` para permitir posicionar elementos internos.
- `nav` usa `display: flex` para alinhar logo, menu e botões em uma linha.
- `.logo` define a largura da imagem do logotipo.
- O menu de navegação usa `nav ul li` e `nav ul li a` para remover marcação padrão e aplicar espaçamento e cor.
- `.login-btn` e `.btn` estilizam os links como botões, com gradiente, borda arredondada e transição suave.
- `.content` limita a largura do texto e adiciona espaçamento superior.
- `.content h1` define um texto grande e visível para o título principal.
- `.content p` define a cor do parágrafo e espaçamento abaixo do texto.
- `.content .btn` aplica padding maior e fonte maior ao botão principal dentro da seção de conteúdo.
- `.recursos-img` posiciona a imagem à direita e embaixo dentro da seção hero.

## Ponto importante

- No CSS, `display: center` não funciona. O correto é usar `display: flex` para alinhar os itens horizontalmente no `nav`.
- A classe `.Logo` no CSS não tinha correspondência com `class="logo"` no HTML. Agora o CSS usa `.logo`.

## Como visualizar

1. Abra o arquivo `index.html` no navegador.
2. Verifique se a pasta `pictures/` está no mesmo diretório e contém as imagens referenciadas.

## Sugestões de melhoria

- Adicionar responsividade com media queries para telas menores.
- Criar animações suaves usando `@keyframes` para entrada dos elementos.
- Ajustar o contraste do texto sobre a imagem de fundo para garantir boa leitura.
