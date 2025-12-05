## 5.1 Ameaças à Validade Interna


### A5.1.1 Viés de Seleção da Fonte de Dados (Ameaça de Amostragem)

**Descrição:**  
Os dados são provenientes exclusivamente de avaliações públicas da Google Play Store. Usuários que publicam avaliações online podem constituir um subgrupo não representativo da população total de usuários, tendendo a ser aqueles com experiências extremamente positivas ou negativas.



**Estratégias de Mitigação:**
- **Transparência Analítica:** Reconhecer explicitamente esta limitação nas conclusões do estudo, qualificando os resultados como representativos da "população de avaliadores", não de todos os usuários.  


---


### A5.1.3 Instrumentação 

**Descrição:**  
Alterações no algoritmo de análise de sentimento (PLN) ou nos critérios de categorização temática durante o processamento dos dados podem introduzir variação não atribuível aos aplicativos ou cidades.

**Categoria:** Viés de medição/instrumentação.

**Estratégias de Mitigação:**
- **Protocolo Operacional Fixo:** Definir e documentar de forma precisa todos os parâmetros, modelos e dicionários de termos a serem utilizados na análise de PLN e categorização antes do início do processamento.  
- **Validação e Consistência:** Aplicar o protocolo completo a um subconjunto de dados de controle em diferentes momentos para verificar a consistência dos resultados.

---

## 5.2 Ameaças à Validade Externa

Ameaças à validade externa referem-se à capacidade de generalizar os resultados do estudo para outros contextos, populações ou momentos.

### A5.2.1 Amostragem Não Probabilística e Especificidade do Contexto

**Descrição:**  
A amostra é composta por todos os dados disponíveis para três aplicativos específicos em três capitais brasileiras durante um período determinado. Isso limita a generalização para outras cidades, outros aplicativos, usuários de outras plataformas (ex.: iOS) ou períodos futuros.

**Categoria:** Validade de população e ecológica.

**Estratégias de Mitigação:**
- **Delimitação Clara do Universo:** Definir e comunicar precisamente o universo da pesquisa.  
- **Descrição Rica do Contexto:** Fornecer uma descrição detalhada dos aplicativos e do contexto urbano das cidades analisadas.  
- **Estrutura Metodológica Replicável:** Documentar a metodologia para que possa ser aplicada em outros estudos comparativos futuramente.

---

## 5.3 Ameaças à Validade de Construto

Ameaças à validade de construto referem-se ao grau em que os procedimentos de medição representam adequadamente os conceitos teóricos em estudo.

### A5.3.1 Operacionalização Incompleta de “Usabilidade”

**Descrição:**  
O estudo opera com o construto de "usabilidade percebida" a partir de avaliações espontâneas. A ISO 9241-11 define três dimensões — eficiência, eficácia e satisfação — que podem não estar completamente refletidas nos comentários dos usuários.

**Categoria:** Validade de medição (viés do construto).

**Estratégias de Mitigação:**
- **Framework de Mapeamento Teórico-Pragmático:** Relacionar tópicos e termos extraídos às dimensões da usabilidade e atributos de qualidade.  
- **Validação por Especialistas:** Enviar amostras classificadas para especialistas em IHC/UX revisarem.  
- **Análise Multimétrica:** Complementar análises de texto com métricas objetivas (ex.: correlação entre nota e sentimento).

---

### A5.3.2 Limitações do Processamento de Linguagem Natural (PLN)

**Descrição:**  
Modelos de PLN podem falhar em sarcasmo, gírias, contexto regional, ironia ou ambiguidade linguística.

**Categoria:** Viés de instrumento/ferramenta.

**Estratégias de Mitigação:**
- **Validação Manual de Subamostra:** Classificar manualmente 10–15% das avaliações para medir acurácia da classificação automática.  
- **Ajuste do Modelo:** Utilizar modelos treinados em português brasileiro e dicionários regionais.  
- **Consistência Cruzada:** Conferir coerência entre sentimento detectado e nota numérica atribuída pelo usuário.

---

## 5.4 Ameaças à Validade Estatística e de Conclusão

### A5.4.1 Poder Estatístico Desbalanceado

**Descrição:**  
O número de avaliações varia entre aplicativos e cidades. Amostras desiguais podem prejudicar comparações e reduzir o poder estatístico.

**Categoria:** Poder do teste / Pressupostos estatísticos.

**Estratégias de Mitigação:**
- **Testes Não Paramétricos:** Usar Kruskal-Wallis, Mann-Whitney, etc.  
- **Análise de Sensibilidade:** Bootstrapping ou subamostragem.  
- **Intervalos de Confiança:** Reportar medidas com ICs, não só valores-p.

---

### A5.4.2 Inferência Causal Inadequada (Natureza Observacional)

**Descrição:**  
O estudo é observacional e não permite atribuição causal entre fatores e resultados.

**Categoria:** Validade de conclusão (inferência causal).

**Estratégias de Mitigação:**
- **Linguagem Cautelosa:** Evitar conclusões causais diretas.  
- **Discussão de Fatores de Confusão:** Identificar variáveis externas possíveis.  
- **Classificação como Estudo Exploratório:** Enfatizar que o objetivo é gerar insights, não provar causalidade.

---

### A5.4.3 Viés do Pesquisador na Análise e Interpretação

**Descrição:**  
Expectativas prévias podem influenciar inconscientemente a análise e interpretação dos dados.

**Categoria:** Viés cognitivo / Validade de conclusão.

**Estratégias de Mitigação:**
- **Análise Exploratória Independente:** Identificar padrões antes de testar hipóteses.  
- **Documentação Auditável:** Manter um log detalhado de todas as decisões metodológicas.  
- **Revisão por Pares:** Submeter resultados a colegas ou orientador.

---
