# 📦 Ana e Leo - MudaLar

> Um catálogo digital rápido, estático e elegante construído para facilitar a venda e repasse de móveis durante uma mudança de cidade.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)

## 📌 Sobre o Projeto

O **MudaLar** nasceu de uma necessidade real: gerenciar a venda de diversos móveis usados de forma organizada, profissional e sem as taxas de plataformas de terceiros. 

Do ponto de vista técnico, é uma **Single Page Application (SPA) estática** focada em performance e facilidade de manutenção. Os dados dos móveis são gerenciados através de um simples arquivo JSON, que é compilado por um script Node.js para ser consumido instantaneamente pelo frontend, eliminando a necessidade de um servidor back-end ou banco de dados em tempo de execução.

## ✨ Funcionalidades

- **Catálogo Dinâmico:** Renderização de dezenas de móveis (fotos, descrição e preço) a partir de uma fonte de dados centralizada.
- **Carrossel de Imagens Customizado:** Galeria de fotos nativa com suporte a *fallback* (imagem padrão caso o item não possua foto).
- **Integração ViaCep API:** Consulta de CEP em tempo real via Fetch API para que o comprador possa calcular a distância e planejar o carreto.
- **Checkout via WhatsApp:** Botões de CTA que capturam os dados do item (nome e valor) e abrem o WhatsApp do vendedor com uma mensagem pré-formatada.
- **Design Utility-First:** Interface 100% responsiva, estilizada com Tailwind CSS via CDN, utilizando variáveis customizadas para uma paleta de cores harmoniosa em tons terrosos.
- **Formulário de Contato:** Interface amigável para recebimento de dúvidas e propostas.

## 🛠️ Arquitetura e Tecnologias

Este projeto foi desenhado para ser simples de hospedar (como no GitHub Pages) e fácil de atualizar.

- **Frontend:** HTML5 semântico, Vanilla JavaScript (sem dependências de frameworks pesados).
- **Estilização:** Tailwind CSS (configurado via script no `<head>` para prototipagem ágil).
- **Tipografia & Ícones:** Google Fonts (EB Garamond, Be Vietnam Pro) e Google Material Symbols.
- **Build/Automação:** Script simples em Node.js (`build-furniture`) que lê o arquivo `furniture.json` e gera o `furniture-data.js` para ser injetado no escopo global da janela (`window`).

## 🚀 Como executar o projeto localmente

Para clonar e rodar esta aplicação no seu ambiente de desenvolvimento (recomendado o uso do editor Cursor ou VS Code), siga os passos:

```bash
# 1. Clone este repositório
$ git clone https://github.com/LisioSouza/mudalar.git

# 2. Acesse a pasta do projeto
$ cd mudalar

# 3. Adicione ou edite os dados dos móveis
# Abra o arquivo assets/furniture.json e faça suas alterações

# 4. Rode o script de build para atualizar a vitrine
$ node scripts/build-furniture.js

# 5. Abra o arquivo index.html no navegador
# Dica: Utilize a extensão "Live Server" para atualização automática em tempo real.
```
## 🌐 Deploy

O projeto está otimizado para ser hospedado gratuitamente no **GitHub Pages**. Basta ir nas configurações (`Settings`) deste repositório, navegar até a aba `Pages`, selecionar a branch `main` e salvar. Em poucos minutos o catálogo estará no ar!

---
Desenvolvido com ☕ e código por [![Lisio Souza](https://img.shields.io/badge/Lisio_Souza-3B82F6?style=flat&logo=github&logoColor=white)](https://github.com/LisioSouza).

_Este projeto foi desenvolvido como requisito de entrega das Atividades 4 e 5 (Construção de Site Simples com HTML, CSS e JS) da [![Formação Desenvolvedor Full Stack Jr](https://img.shields.io/badge/Formação_Desenvolvedor_Full_Stack_Jr-16A34A?style=flat)](#), oferecida pela [+PraTi](https://maisprati.com.br/) em parceria com a [Codifica](https://codificaedu.com.br/) - 2026._
