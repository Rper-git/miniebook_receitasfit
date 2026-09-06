# 🥗 MiniEbook Receitas Fit

## Nutrição Sistêmica, Saciedade e Emagrecimento Saudável

Caderno temático desenvolvido como parte de um Desafio de Projeto da DIO, utilizando pesquisa orientada por fontes e o NotebookLM como ferramenta de apoio ao estudo.

O projeto tem como objetivo investigar conceitos relacionados à alimentação saudável, saciedade, saúde intestinal, planejamento de refeições e preparação prática de alimentos, transformando os conhecimentos estudados em um material de consulta simples e reutilizável.

---

## 🎯 Contexto e Objetivos

### Contexto

A alimentação saudável envolve diferentes fatores que vão além da escolha isolada de alimentos. Este projeto aborda a alimentação de forma sistêmica, considerando aspectos como qualidade dos alimentos, saciedade, densidade energética, organização das refeições e preparação antecipada.

Um dos focos do estudo é a relação entre o intestino e o cérebro, além de estratégias práticas para facilitar a organização alimentar durante a semana.

### Objetivos

Os principais objetivos deste caderno temático são:

1. Compreender conceitos relacionados à relação entre microbiota intestinal e eixo intestino-cérebro.
2. Estudar estratégias de planejamento e preparação antecipada de refeições (Meal Prep).
3. Explorar receitas práticas com atenção à saciedade e à composição nutricional.
4. Investigar substituições de ingredientes com maior densidade energética por alternativas mais leves, quando apropriado.
5. Desenvolver prompts capazes de auxiliar pesquisas, revisões e organização do conhecimento.
6. Transformar o conhecimento obtido em um miniguia de estudo reutilizável.

---

# 📚 Curadoria de Fontes

As fontes utilizadas foram selecionadas considerando sua relevância para os assuntos estudados e foram utilizadas como base para as consultas realizadas no NotebookLM.

| Nº | Fonte                    | Tipo                   | Utilização                                                    |
| -- | ------------------------ | ---------------------- | ------------------------------------------------------------- |
| 1  | Dieta 3 Passos           | Conteúdo especializado | Pesquisa relacionada à alimentação e estratégias nutricionais |
| 2  | TudoGostoso              | Receitas               | Pesquisa e adaptação de preparações                           |
| 3  | Receiteria               | Receitas               | Pesquisa de preparações práticas                              |
| 4  | Materiais especializados | Artigos/Vídeos/PDFs    | Complementação do estudo                                      |

> As fontes devem ser analisadas criticamente e suas informações não devem ser consideradas equivalentes a orientação médica ou nutricional individualizada.

---

# 🧠 Engenharia de Prompts

Durante o desenvolvimento do projeto foram utilizados diferentes tipos de prompts para comparar a qualidade das respostas obtidas.

## Prompt inicial

Um dos primeiros testes utilizou uma abordagem genérica para solicitar sugestões de receitas e estratégias alimentares.

### Problema identificado

As respostas apresentavam informações muito amplas e nem sempre especificavam:

* quantidade de ingredientes;
* objetivo da preparação;
* possibilidade de congelamento;
* substituições de ingredientes;
* modo correto de preparo;
* relação entre os ingredientes e o objetivo da refeição.

---

## Prompt aprimorado

A partir dos problemas encontrados, os prompts passaram a apresentar maior contexto, objetivo e restrições.

Exemplo:

> Atue como um assistente especializado em planejamento de refeições saudáveis. Com base exclusivamente nas fontes disponibilizadas neste notebook, sugira uma preparação prática rica em proteínas e com boa capacidade de saciedade. Informe os ingredientes, quantidades, modo de preparo, possibilidade de congelamento e descongelamento e possíveis substituições. Não invente informações que não estejam presentes nas fontes e indique quando determinada informação não puder ser confirmada.

Essa abordagem produziu respostas mais estruturadas e adequadas ao objetivo do projeto.

---

# 🔎 Cicatrizes e Troubleshooting

Durante os testes foram identificadas algumas dificuldades na interação com a IA.

### 1. Respostas genéricas

Prompts muito curtos produziram respostas superficiais.

**Solução:** fornecer contexto, objetivo, formato esperado e restrições.

### 2. Informações não sustentadas pelas fontes

Algumas respostas poderiam apresentar informações que não estavam claramente presentes no material pesquisado.

**Solução:** solicitar explicitamente que a resposta fosse baseada somente nas fontes disponíveis e que informações não encontradas fossem identificadas como tal.

### 3. Substituições inadequadas

Durante a elaboração das receitas, foi necessário estabelecer critérios para evitar substituições incompatíveis com o objetivo nutricional da preparação.

**Solução:** solicitar alternativas específicas e justificar as substituições com base nas fontes utilizadas.

### 4. Preparação de leguminosas

O preparo de alimentos como feijão e outras leguminosas exigiu atenção especial às etapas de preparo, incluindo o demolho quando recomendado pela fonte utilizada.

**Solução:** solicitar que o modelo descrevesse o procedimento completo de preparação em vez de apresentar apenas a lista de ingredientes.

---

# 📖 Miniguia de Estudo

## 1. Saúde intestinal

A saúde intestinal envolve diferentes aspectos relacionados ao funcionamento do sistema gastrointestinal e à interação entre o intestino e outros sistemas do organismo.

Um dos conceitos estudados neste projeto é o eixo intestino-cérebro, que representa a comunicação bidirecional entre o sistema gastrointestinal e o sistema nervoso.

---

## 2. Planejamento de refeições

O Meal Prep consiste na preparação antecipada de refeições ou componentes das refeições para facilitar a organização alimentar durante a semana.

Entre os aspectos estudados estão:

* planejamento do cardápio;
* organização dos ingredientes;
* preparo em quantidade;
* armazenamento;
* congelamento;
* descongelamento;
* montagem das refeições.

---

## 3. Saciedade e composição das refeições

A composição de uma refeição pode influenciar sua capacidade de proporcionar saciedade.

Neste projeto são estudados especialmente:

* proteínas;
* fibras;
* vegetais;
* sementes;
* aveia;
* alimentos com menor densidade energética.

---

# 📚 Glossário

| Conceito                   | Definição                                                                                          |
| -------------------------- | -------------------------------------------------------------------------------------------------- |
| **Eixo Intestino-Cérebro** | Sistema de comunicação bidirecional entre o trato gastrointestinal e o sistema nervoso.            |
| **Meal Prep**              | Planejamento e preparação antecipada de refeições.                                                 |
| **Densidade Energética**   | Relação entre a quantidade de energia e o peso ou volume de determinado alimento.                  |
| **Pectina**                | Tipo de fibra encontrada principalmente nas paredes celulares de vegetais e frutas.                |
| **Fitatos**                | Compostos presentes em diversos alimentos vegetais que podem interagir com determinados minerais.  |
| **Branqueamento**          | Técnica culinária que utiliza calor por curto período seguida, geralmente, de resfriamento rápido. |
| **Saciedade**              | Sensação de plenitude que contribui para reduzir a necessidade de continuar consumindo alimentos.  |

---

# ♻️ Prompts Reutilizáveis

## Prompt 1 — Análise de receita

> Analise a seguinte receita utilizando exclusivamente as fontes disponíveis. Identifique os principais ingredientes, o método de preparo, possíveis substituições e os aspectos relacionados à saciedade. Não invente informações que não estejam nas fontes.

## Prompt 2 — Meal Prep

> Crie um plano de preparação semanal utilizando as receitas disponíveis nas fontes. Organize as preparações por etapas, indicando quais alimentos podem ser preparados antecipadamente e quais cuidados devem ser considerados para armazenamento, congelamento e descongelamento.

## Prompt 3 — Revisão do conteúdo

> Faça uma revisão do conteúdo estudado neste notebook. Organize os principais conceitos em tópicos, identifique possíveis contradições entre as fontes e indique quais informações precisam de confirmação adicional. Não apresente como fato qualquer informação que não esteja sustentada pelas fontes.

---

# 📝 Conclusão

O desenvolvimento deste caderno permitiu explorar a utilização da Inteligência Artificial como ferramenta de apoio à pesquisa, organização e revisão de conhecimento.

Além do conteúdo relacionado à alimentação e planejamento de refeições, o projeto também possibilitou experimentar técnicas de Engenharia de Prompts, comparar diferentes abordagens e documentar problemas encontrados durante o processo.

O resultado final é um material de estudo que combina curadoria de fontes, experimentação com IA, documentação do processo e organização prática do conhecimento.

