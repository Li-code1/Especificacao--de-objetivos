Especificação de Objetivos (PNL/Coaching)

Este é um projeto simples, criado inteiramente com HTML, CSS e JavaScript Vanilla, que implementa uma ferramenta de **Especificação de Objetivos** baseada em princípios de Programação Neurolinguística (PNL) e Coaching (como o modelo **SMART**).

A ferramenta permite que o usuário defina, de forma estruturada e ecológica, o que deseja alcançar, as evidências de sucesso, os recursos necessários e o primeiro passo prático.

-----

### ✨ Funcionalidades Principais

  * **Formulário Estruturado:** Guia o usuário pela metodologia de especificação de objetivos em blocos: Identificação, Objetivo Específico, Evidências/Prazo, Recursos/Ecologia e Primeiro Passo.
  * **Exportação em PDF:** Permite que o usuário baixe um resumo completo de suas respostas como um documento PDF limpo.
  * **Envio por E-mail (`mailto`):** Gera um rascunho de e-mail com todas as respostas para que o usuário possa enviar o resultado para si mesmo ou para um coach/analista.
  * **Limpar Formulário:** Botão para resetar todos os campos e iniciar uma nova especificação.

-----

### 💻 Tecnologias Utilizadas

| Tecnologia | Descrição |
| :--- | :--- |
| **HTML5** | Estrutura semântica do formulário e interface. |
| **CSS3** | Estilização minimalista e moderna (Dark Theme) para melhor usabilidade. |
| **JavaScript (Vanilla)** | Gerenciamento do estado do formulário e lógica de processamento dos dados. |
| **`jspdf`** | Biblioteca utilizada para a criação do documento PDF. |
| **`dom-to-image-more`** | Biblioteca para transformar a seção de resumo (HTML/CSS) em imagem (PNG) antes de ser inserida no PDF. |

-----

### 🚀 Como Utilizar

Este projeto não requer servidor nem bibliotecas de *build* complexas.

1.  **Clone o repositório:**
    ```bash
    git clone [LINK DO SEU REPOSITÓRIO]
    ```
2.  **Abra o arquivo:**
    Simplesmente abra o arquivo `index.html` (ou o nome que você salvou) em qualquer navegador web moderno.
3.  **Preenchimento:** Preencha os campos seguindo as instruções de cada seção.
4.  **Ações:** Utilize os botões na parte inferior para exportar ou enviar os dados.

> **Configuração:** Para o botão **"Enviar para meu e-mail"** funcionar corretamente no lado do destinatário, altere a constante `TARGET_EMAIL` no arquivo JavaScript para o endereço desejado (atualmente configurado como `lilianelimapsicanalista@gmail.com`).

-----

### ⚙️ Estrutura do Código (Visão Geral)

O código é contido em um único arquivo HTML e segue esta estrutura:

1.  **`<head>`:** Importa as bibliotecas `dom-to-image-more` e `jspdf`.
2.  **`<style>`:** Contém todo o CSS do projeto (incluindo o tema escuro e os ajustes de visualização para o PDF).
3.  **`<body>`:** Contém o `<header>` e a área principal (`<main>`) com o formulário (`<form>`) e a área oculta de preview (`#previewForPdf`).
4.  **`<script>`:** Contém toda a lógica JavaScript, incluindo as funções de:
      * `updateState()`: Coleta os dados dos inputs.
      * `updatePreview()`: Atualiza a área oculta que será capturada no PDF.
      * Ações dos botões (`sendEmailBtn`, `downloadPdfBtn`, `resetBtn`).

-----

### 🤝 Contribuições

Contribuições, sugestões de melhoria no layout ou otimizações no código JavaScript (especialmente na parte de geração do PDF) são bem-vindas\! Sinta-se à vontade para abrir uma *Issue* ou enviar um *Pull Request*.
