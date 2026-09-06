# 🧠 Engenharia de Prompts

Durante a elaboração do MiniEbook Receitas Fit, foram realizados diferentes testes com prompts no NotebookLM.

O objetivo dos testes foi observar como a qualidade das instruções fornecidas ao modelo poderia influenciar a organização, profundidade e utilidade das respostas.

---

## 1. Primeiro teste — Prompt genérico

### Prompt utilizado

> Me passe receitas fit para emagrecer.

### Resultado observado

A resposta apresentou sugestões gerais de receitas, porém sem especificar adequadamente critérios como:

* quantidade dos ingredientes;
* modo de preparo;
* quantidade de porções;
* possibilidade de congelamento;
* substituições;
* organização semanal;
* relação com as fontes utilizadas.

### Problema identificado

O prompt apresentava pouco contexto e não definia claramente o formato da resposta esperado.

---

## 2. Segundo teste — Inclusão de contexto

### Prompt utilizado

> Quero criar um mini eBook de receitas fit para pessoas que procuram opções práticas para organizar a alimentação durante a semana. Sugira receitas fáceis, com ingredientes acessíveis e que possam ser preparadas antecipadamente.

### Resultado observado

A resposta apresentou sugestões mais próximas do objetivo do projeto.

Entretanto, ainda havia informações genéricas e algumas sugestões não estavam necessariamente relacionadas às fontes selecionadas.

### Problema identificado

O modelo precisava receber instruções mais específicas sobre as fontes que deveriam ser utilizadas.

---

## 3. Terceiro teste — Restringindo as fontes

### Prompt utilizado

> Com base exclusivamente nas fontes disponíveis neste notebook, identifique receitas que sejam adequadas para um mini eBook de alimentação saudável. Para cada receita, apresente o nome, ingredientes, modo de preparo e a fonte utilizada. Não invente receitas ou informações que não estejam presentes nas fontes.

### Resultado observado

A resposta tornou-se mais organizada e passou a relacionar as informações às fontes disponibilizadas.

### Melhoria identificada

A utilização da expressão **"com base exclusivamente nas fontes disponíveis"** ajudou a reduzir respostas que poderiam extrapolar o material de pesquisa.

---

## 4. Quarto teste — Meal Prep

### Prompt utilizado

> Atue como um assistente especializado em organização de refeições. Com base nas fontes disponíveis neste notebook, selecione preparações adequadas para Meal Prep. Organize as receitas considerando preparo antecipado, porcionamento, armazenamento, congelamento e descongelamento. Quando uma informação não estiver disponível nas fontes, informe explicitamente que ela não foi encontrada.

### Resultado observado

A resposta passou a apresentar as receitas dentro de um contexto mais prático de organização semanal.

Também foi possível identificar quais informações estavam efetivamente disponíveis nas fontes e quais precisariam de confirmação adicional.

---

## 5. Quinto teste — Criação de receita estruturada

### Prompt utilizado

> Analise as receitas presentes nas fontes e selecione uma preparação adequada para o mini eBook. Apresente a resposta na seguinte estrutura:
>
> 1. Nome da receita
> 2. Objetivo da preparação
> 3. Ingredientes
> 4. Quantidades
> 5. Modo de preparo
> 6. Rendimento
> 7. Armazenamento
> 8. Possibilidade de congelamento
> 9. Substituições possíveis
> 10. Fonte original
>
> Utilize somente informações que possam ser identificadas nas fontes. Caso alguma informação não esteja disponível, escreva "não informado na fonte".

### Resultado observado

A estrutura da resposta tornou-se mais consistente e facilitou a transformação das informações pesquisadas em conteúdo para o eBook.

---

# 📊 Comparação dos testes

| Teste | Estratégia                          | Resultado                                      |
| ----- | ----------------------------------- | ---------------------------------------------- |
| 01    | Prompt genérico                     | Resposta ampla e superficial                   |
| 02    | Inclusão de contexto                | Melhor compreensão do objetivo                 |
| 03    | Restrição às fontes                 | Maior rastreabilidade                          |
| 04    | Definição de critérios de Meal Prep | Respostas mais práticas                        |
| 05    | Estrutura detalhada                 | Respostas organizadas para utilização no eBook |

---

# 🎯 Principais aprendizados

Os testes demonstraram que prompts mais eficientes normalmente apresentam:

* contexto;
* objetivo;
* público-alvo;
* fontes que devem ser utilizadas;
* critérios de seleção;
* formato esperado da resposta;
* limitações;
* instruções para não inventar informações.

A evolução dos prompts permitiu transformar perguntas genéricas em instruções mais estruturadas e adequadas ao objetivo do projeto.

---

# ♻️ Princípio utilizado

Uma das principais estratégias adotadas foi:

**Contexto + Objetivo + Fonte + Restrições + Formato de resposta**

Essa estrutura pode ser reutilizada em futuras pesquisas realizadas com ferramentas de Inteligência Artificial.
