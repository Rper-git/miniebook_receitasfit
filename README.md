# 🥗 MiniEbook Receitas Fit

## Nutrição Sistêmica, Saciedade e Emagrecimento Saudável

Caderno temático desenvolvido como parte de um **Desafio de Projeto da DIO**, utilizando curadoria de fontes, experimentação de prompts e o **NotebookLM** como ferramenta de apoio à pesquisa, organização e análise do conhecimento.

O projeto reúne receitas práticas, estratégias de **Meal Prep**, organização alimentar e conceitos relacionados à saciedade e saúde intestinal, documentando também o processo de utilização da Inteligência Artificial.

---

## 🎯 Contexto e Objetivos

### Contexto

A alimentação saudável envolve diferentes fatores que vão além da escolha isolada de alimentos.

Este projeto aborda o tema de forma integrada, considerando:

* composição das refeições;
* variedade alimentar;
* saciedade;
* densidade energética;
* preparação dos alimentos;
* organização semanal;
* Meal Prep;
* armazenamento e congelamento;
* adaptação de receitas.

Um dos temas estudados é a relação entre o intestino e o cérebro, juntamente com estratégias práticas para facilitar a organização alimentar durante a semana.

### Objetivos

Os principais objetivos são:

1. Estudar conceitos relacionados à alimentação, saciedade e saúde intestinal.
2. Explorar estratégias de planejamento e preparação antecipada de refeições.
3. Organizar receitas práticas encontradas nas fontes selecionadas.
4. Analisar possibilidades de adaptação e substituição de ingredientes.
5. Experimentar diferentes técnicas de Engenharia de Prompts.
6. Documentar problemas encontrados durante a utilização da IA e suas respectivas soluções.
7. Transformar o conhecimento pesquisado em um miniguia de estudo reutilizável.

---

## 📚 Curadoria de Fontes

Foram selecionadas **9 fontes**, divididas entre portais de receitas e vídeos sobre receitas, Meal Prep e organização alimentar.

As fontes completas e suas respectivas contribuições estão documentadas em:

➡️ [`fontes/fontes.md`](fontes/fontes.md)

### Resumo das fontes

| Nº | Fonte                  | Tipo               | Principal contribuição                          |
| -- | ---------------------- | ------------------ | ----------------------------------------------- |
| 1  | Dieta 3 Passos         | Portal de receitas | Receitas fitness e adaptações                   |
| 2  | TudoGostoso            | Portal de receitas | Receitas e preparações práticas                 |
| 3  | Receiteria             | Portal de receitas | Receitas fitness simples                        |
| 4  | Betto Auge             | Vídeo              | Torta de frango fit e preparação proteica       |
| 5  | Anjo Low Carb Receitas | Vídeo              | Preparações de forno e receitas low carb        |
| 6  | Itaciária Cordeiro     | Vídeo              | Receitas saudáveis e rápidas                    |
| 7  | Doobydobap             | Vídeo              | Meal Prep e saúde intestinal                    |
| 8  | Mirielly Ruback        | Vídeo              | Preparação de proteínas e alimentos congeláveis |
| 9  | Gabi Barreto           | Vídeo              | Marmitas, preparação em volume e congelamento   |

> As fontes práticas foram utilizadas principalmente para receitas, técnicas culinárias e organização alimentar. Informações relacionadas à saúde e nutrição devem ser interpretadas de acordo com a fonte original e, quando necessário, confrontadas com literatura científica e orientação profissional.

---

## 🧠 Engenharia de Prompts

Durante o desenvolvimento foram realizados diferentes testes de prompts para avaliar como a qualidade das instruções influencia os resultados produzidos pela IA.

O processo começou com perguntas genéricas e evoluiu para prompts com:

* contexto;
* objetivo;
* fontes;
* critérios;
* formato de resposta;
* limitações;
* instruções de verificação.

Os testes completos estão documentados em:

➡️ [`prompts/prompts-testados.md`](prompts/prompts-testados.md)

### Estrutura utilizada

**Contexto + Objetivo + Fontes + Critérios + Formato + Limitações**

Essa estrutura ajudou a reduzir respostas genéricas e aumentar a rastreabilidade das informações.

---

## 🔎 Cicatrizes e Troubleshooting

Durante o desenvolvimento foram identificados problemas relacionados à utilização da Inteligência Artificial, incluindo:

* respostas genéricas;
* informações não encontradas nas fontes;
* substituições de ingredientes;
* preparo incompleto de receitas;
* dúvidas sobre congelamento e descongelamento;
* generalização de técnicas culinárias;
* interpretação de informações nutricionais;
* confusão entre conteúdo culinário e evidência científica.

Para cada problema foram testadas estratégias de reformulação dos prompts.

A documentação completa está disponível em:

➡️ [`prompts/cicatrizes.md`](prompts/cicatrizes.md)

### Processo utilizado

**Pesquisar → Testar → Identificar problemas → Reformular → Verificar → Documentar**

---

## 📖 Miniguia de Estudo

O projeto também resultou em um miniguia organizado por temas.

Entre os principais assuntos estão:

* Nutrição Sistêmica;
* eixo intestino-cérebro;
* saciedade;
* densidade energética;
* Meal Prep;
* preparação em grande volume;
* congelamento;
* branqueamento de vegetais;
* leguminosas;
* proteínas;
* fibras;
* substituição de ingredientes;
* organização semanal.

➡️ [`miniguia/resumo.md`](miniguia/resumo.md)

---

## 📚 Glossário

Foi criado um glossário com os principais termos utilizados durante a pesquisa, incluindo:

* microbiota;
* eixo intestino-cérebro;
* saciedade;
* densidade energética;
* Meal Prep;
* branqueamento;
* pectina;
* fitatos;
* leguminosas;
* fibras;
* porcionamento;
* Engenharia de Prompts;
* NotebookLM.

➡️ [`miniguia/glossario.md`](miniguia/glossario.md)

---

## 🤖 Prompts Reutilizáveis

Como resultado da experimentação, foram criados prompts que podem ser reutilizados em futuras pesquisas.

Eles incluem modelos para:

* pesquisa baseada em fontes;
* análise de receitas;
* planejamento de Meal Prep;
* comparação de receitas;
* identificação de adaptações;
* análise de congelamento;
* estudo de conceitos;
* melhoria de prompts;
* verificação crítica de respostas;
* utilização de um prompt mestre.

➡️ [`miniguia/prompts-reutilizaveis.md`](miniguia/prompts-reutilizaveis.md)

---

## 📁 Estrutura do Repositório

```text
miniebook_receitasfit/
│
├── README.md
│
├── fontes/
│   └── fontes.md
│
├── prompts/
│   ├── prompts-testados.md
│   └── cicatrizes.md
│
└── miniguia/
    ├── resumo.md
    ├── glossario.md
    └── prompts-reutilizaveis.md
```

---

## 🛠️ Ferramentas Utilizadas

* **GitHub** — organização e versionamento do projeto.
* **NotebookLM** — apoio na análise e consulta das fontes selecionadas.
* **Inteligência Artificial** — experimentação, organização e revisão do conteúdo.
* **Markdown** — documentação dos materiais.

---

## 📌 Principais Aprendizados

O desenvolvimento deste projeto permitiu compreender que uma boa pesquisa com Inteligência Artificial depende de mais do que simplesmente fazer perguntas.

Foi necessário:

1. Selecionar fontes relevantes.
2. Organizar os materiais.
3. Criar prompts específicos.
4. Comparar diferentes respostas.
5. Identificar limitações.
6. Verificar informações.
7. Diferenciar fontes práticas de informações científicas.
8. Documentar o processo.

O projeto também demonstrou a importância da **rastreabilidade**, evitando apresentar como informação de uma fonte algo que não esteja efetivamente presente nela.

---

## ⚠️ Considerações

Este projeto possui finalidade **educacional e de estudo**.

Os conteúdos apresentados não substituem avaliação, orientação ou acompanhamento de profissionais de saúde.

Receitas, vídeos e portais utilizados como fontes práticas não devem ser automaticamente interpretados como evidência científica.

---

## 📝 Conclusão

O **MiniEbook Receitas Fit** reúne pesquisa, curadoria de fontes, Engenharia de Prompts, experimentação com Inteligência Artificial e organização do conhecimento.

O resultado é um caderno temático que não apenas apresenta informações sobre receitas e organização alimentar, mas também demonstra **como o conhecimento foi pesquisado, estruturado, verificado e documentado com o auxílio da IA**.

---

## 👤 Autor

**Robson**

Projeto desenvolvido para o **Desafio de Projeto da DIO**.

---

⭐ Projeto desenvolvido com foco em **aprendizado, organização do conhecimento e experimentação prática com Inteligência Artificial**.
