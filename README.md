<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Poppins&color=FF4500&size=24&center=true&vCenter=true&width=600&lines=Delivery+Senac+🍕;Sistema+de+Pedidos+Online;Cardápio+Dinâmico;Carrinho+de+Compras+Interativo" />
</p>

---

# Delivery Senac — Sistema de Pedidos de Pizzaria

Sistema de pedidos online de uma pizzaria, desenvolvido em sala de aula durante o início do Curso Técnico em Informática para Internet no Senac Lapa Tito. O projeto simula um cardápio digital com carrinho de compras funcional e cadastro de novos produtos.

---

> **Aviso**
>
> Este repositório é **exclusivamente para fins educacionais**.
> O projeto foi desenvolvido em sala de aula como exercício prático e pode conter
> implementações simplificadas ou inacabadas, condizentes com o nível introdutório da atividade.

---

## Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Funcionalidades](#funcionalidades)
- [Tecnologias](#tecnologias)
- [Estrutura de Arquivos](#estrutura-de-arquivos)
- [Como Executar](#como-executar)
- [Cardápio Disponível](#cardápio-disponível)
- [Aprendizados](#aprendizados)
- [Autor](#autor)

---

## Sobre o Projeto

O Delivery Senac é uma aplicação front-end que simula o funcionamento de um sistema de pedidos de pizzaria. O usuário consegue visualizar o cardápio completo, adicionar pizzas ao carrinho, remover itens e acompanhar o valor total do pedido em tempo real.

O projeto também conta com um modal de cadastro que permite adicionar novas pizzas ao cardápio dinamicamente, sem recarregar a página.

Todo o cardápio é gerado via JavaScript, manipulando o DOM diretamente — sem frameworks ou bibliotecas de UI externas.

---

## Funcionalidades

- Exibição dinâmica do cardápio gerado via JavaScript
- Adição de pizzas ao carrinho com alerta de confirmação
- Remoção de itens individuais do carrinho
- Cálculo e exibição do valor total em tempo real
- Modal de cadastro de novas pizzas com campos de nome, foto, valor e ingredientes
- Carrinho com animação de entrada e saída (slide)
- Modal com animação de abertura e fechamento (fade)
- Layout responsivo para telas de até 425px

---

## Tecnologias

| Tecnologia | Uso |
|---|---|
| HTML5 | Estrutura da página e elemento `<dialog>` nativo para o modal |
| CSS3 | Estilização, animações com `@keyframes` e responsividade |
| JavaScript (ES6) | Manipulação do DOM, eventos, arrays e funções |
| Google Fonts | Família tipográfica Poppins |
| JSON | Estrutura de dados do cardápio (`pizza.json`) |

---

## Estrutura de Arquivos

```
DeliverySenac/
│
├── index.html
│
├── pizza.json
│
├── css/
│   ├── delivery.css
│   └── modal.css
│
├── js/
│   ├── pizzas.js
│   ├── cardapio.js
│   ├── carrinho.js
│   └── app.js
│
└── imgs/
    ├── pizza-de-calabresa.jpg
    ├── pizza-de-frango-com-catupiry.jpg
    ├── pizza-de-mussarela.jpg
    ├── pizza-de-portuguesa.jpg
    ├── pizza-de-bacon.jpg
    ├── pizza-de-marguerita.webp
    ├── pizza-de-pepperoni.jpg
    └── pizza-de-brigadeiro.jpg
```

### Responsabilidade de cada arquivo

| Arquivo | Responsabilidade |
|---|---|
| `index.html` | Estrutura da página, navegação, cardápio, carrinho e modal |
| `delivery.css` | Estilização geral, carrinho, navegação e responsividade |
| `modal.css` | Estilização e animações do modal de cadastro |
| `pizzas.js` | Array com os dados iniciais do cardápio |
| `cardapio.js` | Função `exibirCardapio()` — renderiza as pizzas no DOM |
| `carrinho.js` | Função `atualizarCarrinho()` — gerencia itens e total |
| `app.js` | Eventos gerais: abrir/fechar carrinho, modal e cadastro de pizza |
| `pizza.json` | Estrutura de dados do cardápio em formato JSON |

---

## Como Executar

Não há dependências de instalação. O projeto roda diretamente no navegador.

**1. Clone o repositório**
```bash
git clone https://github.com/samuelftc/deliverysenac.git
```

**2. Acesse a pasta do projeto**
```bash
cd deliverysenac
```

**3. Abra no navegador**

Abra o arquivo `index.html` diretamente no navegador, ou use a extensão **Live Server** no VS Code para um ambiente de desenvolvimento local.

> As imagens das pizzas devem estar na pasta `imgs/` com os nomes exatos referenciados no arquivo `pizzas.js`.

---

## Cardápio Disponível

| Pizza | Ingredientes | Valor |
|---|---|---|
| Calabresa | Calabresa, cebola, mussarela | R$ 50,00 |
| Frango com Catupiry | Frango, catupiry, mussarela | R$ 60,00 |
| Mussarela | Molho, mussarela | R$ 50,00 |
| Portuguesa | Ovo, presunto, mussarela, molho | R$ 60,00 |
| Bacon | Bacon, mussarela, molho | R$ 70,00 |
| Marguerita | Molho, manjericão, mussarela, tomate | R$ 50,00 |
| Pepperoni | Pepperoni, mussarela | R$ 70,00 |
| Brigadeiro | Creme de chocolate, brigadeiro | R$ 45,00 |

---

## Aprendizados

Este projeto consolidou os seguintes conceitos:

- **Manipulação do DOM** criando, inserindo e removendo elementos HTML via JavaScript puro
- **Eventos (`addEventListener`)** para interações de clique em botões dinâmicos
- **Arrays e métodos** como `push()`, `splice()`, `indexOf()`, `forEach()` e `join()`
- **Funções reutilizáveis** como `exibirCardapio()` e `atualizarCarrinho()` chamadas em múltiplos pontos
- **Elemento `<dialog>`** nativo do HTML5 para criação de modal sem JavaScript extra
- **Animações CSS** com `@keyframes` para slide do carrinho e fade do modal
- **Separação de responsabilidades** dividindo o código em arquivos com funções específicas
- **Estrutura de dados com JSON** e como ela se relaciona com o array de objetos em JavaScript
- **`parseFloat()` e `.toFixed(2)`** para trabalhar com valores monetários
- **Responsividade básica** com media queries para dispositivos móveis

---

## Autor

Desenvolvido por **Samuel Ferreira**

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Samuelftc)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:samuelferreiradev08@gmail.com)

---

> Projeto desenvolvido como atividade prática no **Curso Técnico em Informática para Internet — Senac**.
