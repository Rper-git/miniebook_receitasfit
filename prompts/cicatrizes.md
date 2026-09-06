# 🔎 Cicatrizes e Troubleshooting

Durante o desenvolvimento do MiniEbook Receitas Fit, foram identificadas algumas dificuldades na utilização da Inteligência Artificial para interpretar fontes, selecionar receitas e transformar as informações em conteúdo estruturado.

Esta seção documenta os principais problemas encontrados e as estratégias utilizadas para melhorar os resultados.

---

## 1. Respostas muito genéricas

### Problema

Nos primeiros testes, prompts curtos como:

> "Me passe receitas fit para emagrecer."

produziram respostas muito amplas.

As sugestões não apresentavam necessariamente critérios claros de seleção, fonte de origem ou informações suficientes para utilização no eBook.

### Solução

O prompt passou a informar:

* objetivo do projeto;
* tipo de receita desejada;
* fontes disponíveis;
* público-alvo;
* formato da resposta;
* restrições.

### Aprendizado

Quanto mais claro o objetivo, maior a possibilidade de obter uma resposta adequada à finalidade do projeto.

---

# 2. Informações que não estavam nas fontes

### Problema

Durante a pesquisa, algumas respostas poderiam apresentar informações adicionais que não estavam claramente presentes nos materiais fornecidos ao NotebookLM.

Isso poderia comprometer a rastreabilidade do conteúdo.

### Solução

Foi adicionada uma instrução específica:

> "Utilize somente informações presentes nas fontes. Caso uma informação não esteja disponível, informe que ela não foi encontrada."

### Aprendizado

Restringir o modelo às fontes selecionadas ajuda a diferenciar o que foi encontrado na pesquisa daquilo que poderia ser uma complementação externa.

---

# 3. Substituições de ingredientes

### Problema

Durante a criação e adaptação das receitas, algumas sugestões de substituição poderiam alterar significativamente a composição da preparação.

Um exemplo foi a utilização de ingredientes lácteos com maior teor de gordura quando o objetivo da receita era utilizar uma alternativa mais leve.

### Solução

Os prompts passaram a solicitar que as substituições fossem apresentadas separadamente e que o modelo não criasse substituições sem suporte nas fontes.

Exemplo de instrução:

> "Ao sugerir uma substituição, informe se ela está presente nas fontes utilizadas. Caso não esteja, identifique a sugestão como uma adaptação e não como informação original da fonte."

### Aprendizado

É importante diferenciar:

**Receita original → adaptação → sugestão do modelo.**

Essa separação evita atribuir à fonte uma informação que foi criada ou modificada durante o processo.

---

# 4. Preparação de leguminosas

### Problema

As etapas de preparo de leguminosas exigem mais detalhes do que simplesmente informar o tempo de cozimento.

Durante a organização do conteúdo, foi necessário prestar atenção às etapas relacionadas ao preparo e ao demolho quando indicado pela fonte.

### Solução

Foi solicitado que o modelo apresentasse o processo completo e identificasse quais etapas estavam efetivamente descritas na fonte.

### Aprendizado

Para instruções culinárias, prompts que solicitam o procedimento completo tendem a produzir informações mais úteis do que perguntas que pedem apenas uma receita resumida.

---

# 5. Congelamento e descongelamento

### Problema

Nem todas as receitas possuem o mesmo comportamento após congelamento e descongelamento.

Alguns alimentos podem alterar textura, consistência ou aparência.

### Solução

Os prompts passaram a solicitar informações específicas sobre:

* possibilidade de congelamento;
* armazenamento;
* descongelamento;
* textura após o descongelamento;
* necessidade de preparação prévia.

Quando a fonte não apresentava determinada informação, ela deveria ser identificada como "não informado na fonte".

### Aprendizado

O fato de uma receita ser saudável ou prática não significa automaticamente que ela seja adequada para congelamento.

---

# 6. Preparação de massas para congelamento

### Problema

Durante a pesquisa de Meal Prep, surgiu a necessidade de considerar o comportamento das massas após congelamento e descongelamento.

O cozimento excessivo pode comprometer a textura final da preparação.

### Solução

A informação encontrada nas fontes foi registrada separadamente, evitando transformar uma técnica apresentada em um vídeo específico em uma regra universal para todas as massas.

### Aprendizado

Uma técnica culinária apresentada em uma fonte deve ser contextualizada antes de ser generalizada para outras preparações.

---

# 7. Informações nutricionais

### Problema

Receitas podem apresentar valores nutricionais, como calorias e quantidade de proteínas, mas esses números dependem dos ingredientes, marcas, quantidades e método de cálculo.

### Solução

Os valores apresentados nas fontes foram tratados como informações da própria fonte, evitando apresentá-los como valores universais.

### Aprendizado

Informações nutricionais devem ser contextualizadas e, quando necessário, verificadas por meio de fontes especializadas.

---

# 8. Confusão entre conteúdo culinário e evidência científica

### Problema

Algumas fontes utilizadas no projeto são vídeos e portais de receitas. Esses materiais são úteis para técnicas culinárias e ideias de preparações, mas não devem ser automaticamente tratados como evidência científica.

### Solução

O projeto passou a separar:

### Fontes práticas

Utilizadas para:

* receitas;
* técnicas culinárias;
* organização de refeições;
* Meal Prep;
* congelamento.

### Fontes conceituais

Utilizadas para:

* conceitos de saúde;
* fisiologia;
* microbiota;
* relação intestino-cérebro;
* aspectos nutricionais.

### Aprendizado

A qualidade da pesquisa depende não apenas da quantidade de fontes, mas também da adequação de cada fonte ao tipo de informação que se deseja obter.

---

# 📌 Síntese das principais cicatrizes

| Problema                             | Solução                               |
| ------------------------------------ | ------------------------------------- |
| Respostas genéricas                  | Aumentar o contexto do prompt         |
| Informações não presentes nas fontes | Restringir a resposta às fontes       |
| Substituições inadequadas            | Solicitar e identificar adaptações    |
| Preparo incompleto                   | Solicitar o procedimento completo     |
| Congelamento sem contexto            | Solicitar informações específicas     |
| Generalização de técnicas            | Contextualizar a informação           |
| Valores nutricionais                 | Identificar a origem dos valores      |
| Mistura entre receitas e ciência     | Separar fontes práticas e conceituais |

---

# 🎯 Principal aprendizado

O principal aprendizado durante o desenvolvimento foi perceber que a qualidade da resposta não depende apenas da ferramenta de Inteligência Artificial.

A qualidade do resultado também está relacionada à qualidade das fontes, à clareza das instruções, às restrições estabelecidas e à capacidade de analisar criticamente a resposta produzida.

O processo passou a seguir uma lógica de:

**Pesquisar → Testar → Identificar problemas → Reformular → Verificar → Documentar.**
