# Portfólio Pessoal

**Aluna:** Thaina Rodrigues de Almeida
**Curso:** Técnico em Desenvolvimento de Sistemas (ETEC), Agenda 15 de Desenvolvimento de Sistemas I

## Descrição

Site de portfólio pessoal que apresenta meu perfil profissional, minhas habilidades, minha trajetória e os projetos que desenvolvi no curso. Ele une as duas áreas em que atuo: biomedicina (laboratório e pesquisa) e tecnologia (desenvolvimento e nuvem).

## Link do site publicado

https://thaina30.github.io/portfolio/


## Tecnologias utilizadas

- HTML5
- CSS3 (variáveis, media queries)
- Bootstrap 5.3.3
- JavaScript
- Devicon (ícones)
- GitHub e GitHub Pages

## Como o projeto funciona

O site é uma página única (`index.html`) com as seguintes partes:

1. **Menu de navegação:** barra fixa no topo, responsiva, com links internos para cada seção.
2. **Carousel:** três slides de abertura, criados só com CSS, com botões que levam às seções.
3. **Perfil:** apresentação, formação, localização e objetivo, organizados em cards.
4. **Habilidades:** cards separados por área, com filtro interativo (recurso novo).
5. **Trajetória:** linha do tempo com a experiência profissional.
6. **Projetos:** cards com atividades feitas no curso.
7. **Contato:** botões para e-mail, GitHub e LinkedIn.
8. **Rodapé.**

## Recurso novo adicionado

**Seção de Habilidades com filtro interativo**, além de uma seção de Trajetória em linha do tempo e de um carousel com slides feitos em CSS, o que melhora o layout em relação ao modelo da aula.

O visitante escolhe entre **Todas**, **Laboratório** e **Tecnologia**, e a página mostra só as habilidades daquela área.

## Como o recurso foi implementado

- Cada card de habilidade recebeu o atributo `data-area` com o valor `lab` ou `tech`.
- Os três botões do filtro têm o atributo `data-filtro` com o valor que representam (`todas`, `lab` ou `tech`).
- Um pequeno script em JavaScript escuta o clique de cada botão, marca o botão ativo e, para cada card, compara `data-area` com o filtro escolhido.
- Os cards que não correspondem recebem a classe `oculta`, que no CSS aplica `display: none`.
- As cores da página ficam em variáveis CSS (`:root`), e as animações respeitam `prefers-reduced-motion`.

## Como executar localmente

1. Baixe ou clone o repositório.
2. Abra o arquivo `index.html` no navegador.

## Publicação

O site foi publicado com o GitHub Pages (Settings > Pages > Branch `main` > pasta `/root`).