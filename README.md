# Protótipo de IA para Geração de Relatórios (Desafio 2 - Business Case Gocase)

Este repositório contém a documentação e o código-fonte da solução proposta para o Desafio 2 do Business Case da Gocase, focado na aplicação prática de Inteligência Artificial para otimizar um processo da área de dados.

---

## 1. O Problema: A Distância entre Dados e Decisões

No ambiente dinâmico de um e-commerce, dados são gerados a cada segundo. Embora dashboards e planilhas sejam ferramentas poderosas, eles ainda exigem que os tomadores de decisão (gerentes, diretores) invistam tempo e conhecimento técnico para extrair insights.

O principal desafio identificado é a "última fronteira" da análise de dados: a tradução de tabelas e números complexos em um resumo claro, rápido e em linguagem natural que possa ser consumido em menos de um minuto e que impulsione ações estratégicas.

## 2. A Solução: Um "Analista de Dados Júnior" Automatizado

A solução proposta é um protótipo de **Gerador de Relatórios Diários com IA**, construído em Google Sheets e integrado com a API do Google Gemini.

Este sistema funciona como um "analista de dados júnior" automatizado, capaz de:
-   Receber um conjunto de dados de vendas diárias.
-   Analisar os dados com base em um conjunto de instruções (prompt).
-   Gerar um sumário executivo em texto, destacando os principais KPIs, tendências e pontos de atenção.

O resultado final é um insight de alto valor, comunicado de forma clara e acessível para qualquer pessoa na empresa, independentemente de sua familiaridade com análise de dados.

### Vantagens da Solução:
-   **Agilidade:** Reduz o tempo de análise de horas para segundos.
-   **Democratização:** Torna os insights dos dados acessíveis a todos.
-   **Integração:** O output (texto) é universal e pode ser facilmente integrado a outros sistemas para enviar relatórios automáticos por e-mail, Slack ou outros canais de comunicação.

---

## 3. Como Usar o Protótipo

O protótipo foi desenvolvido em **Google Sheets** para facilitar a demonstração. Siga os passos abaixo para testá-lo:

**Pré-requisitos:**
-   Uma Conta Google.
-   Uma chave de API do Google AI Studio (Gemini). É possível obter uma gratuitamente em [aistudio.google.com](https://aistudio.google.com/).

**Passos:**

1.  **Crie uma cópia da Planilha:**
    * *<ins>https://docs.google.com/spreadsheets/d/1GeMojZtI8ZhBl6m7-AzUqeQbvF0qtY5F6tO38ZXQW1c/edit?usp=sharing</ins>*

2.  **Configure a Aba de Dados (`Dados_Vendas_Diarias`):**
    * Navegue até a primeira aba. Ela contém uma tabela com os dados de exemplo. Você pode modificar os valores de `unidades_vendidas` e `faturamento` para ver como a IA reage a diferentes cenários.

3.  **Configure o Script de IA:**
    * No menu, vá em **Extensões > Apps Script**.
    * No editor de script que se abrir, localize a linha: `const apiKey = "SUA_CHAVE_API_AQUI";`
    * Substitua `"SUA_CHAVE_API_AQUI"` pela sua chave de API do Google AI Studio que você gerou.
    * Salve o projeto clicando no ícone de disquete.

4.  **Execute a Análise:**
    * Volte para a planilha e navegue até a aba **`Dashboard_Relatorio`**.
    * Clique no botão **"Gerar Relatório"**.
    * Na primeira vez que executar, o Google pedirá sua autorização para que o script possa acessar a planilha e se conectar a serviços externos. Conceda as permissões necessárias.
    * Aguarde alguns segundos e o relatório gerado pela IA aparecerá na célula designada.

---

## 4. Tecnologias Utilizadas

-   **Plataforma de Protótipo:** Google Sheets
-   **Motor de Automação:** Google Apps Script
-   **Inteligência Artificial:** API do Google Gemini (modelo `gemini-2.0-flash-latest`)

---

## 5. Autor

**[Rodrigo da Silva Carvalho Maia]**

-   [https://www.linkedin.com/in/rodrigo-maia-2747861a3]
-   [https://github.com/RodrigoMaia03]
