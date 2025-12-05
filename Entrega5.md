## 5.1 Ameaças à Validade Interna


### A5.1.1 Viés de Seleção da Fonte de Dados 

**Descrição:**  
Os dados são provenientes exclusivamente de avaliações públicas da Google Play Store. Usuários que publicam avaliações online podem constituir um subgrupo não representativo da população total de usuários, tendendo a ser aqueles com experiências extremamente positivas ou negativas.



**Estratégias de Mitigação:**
- **Transparência Analítica:** Reconhecer explicitamente esta limitação nas conclusões do estudo, qualificando os resultados como representativos da "população de avaliadores", não de todos os usuários.  


---


### A5.1.2 Instrumentação 

**Descrição:**  
Alterações no algoritmo de análise de sentimento (PLN) ou nos critérios de categorização temática durante o processamento dos dados podem introduzir variação não atribuível aos aplicativos ou cidades.


**Estratégias de Mitigação:**
- **Protocolo Operacional Fixo:** Definir e documentar de forma precisa todos os parâmetros, modelos e dicionários de termos a serem utilizados na análise de PLN e categorização antes do início do processamento.  
- **Validação e Consistência:** Aplicar o protocolo completo a um subconjunto de dados de controle em diferentes momentos para verificar a consistência dos resultados.

---


## 5.2 Ameaças à Validade de Construto



### A5.3.1 Percepção de “Usabilidade”

**Descrição:**  
O estudo opera com o construto de "usabilidade percebida" a partir de avaliações espontâneas. A ISO 9241-11 define três dimensões — eficiência, eficácia e satisfação — que podem não estar completamente refletidas nos comentários dos usuários.


**Estratégias de Mitigação:**
- **Framework de Mapeamento Teórico-Pragmático:** Relacionar tópicos e termos extraídos às dimensões da usabilidade e atributos de qualidade.  
- **Validação por Especialistas:** Enviar amostras classificadas para especialistas em IHC/UX revisarem.  
- **Análise Multimétrica:** Complementar análises de texto com métricas objetivas (ex.: correlação entre nota e sentimento).

---


## 5.4 Ameaças à Validade Estatística e de Conclusão


### A5.4.1 Viés na Análise e Interpretação

**Descrição:**  
Expectativas prévias podem influenciar inconscientemente a análise e interpretação dos dados.

**Categoria:** Viés cognitivo / Validade de conclusão.

**Estratégias de Mitigação:**
- **Análise Exploratória Independente:** Identificar padrões antes de testar hipóteses.  
- **Documentação Auditável:** Manter um log detalhado de todas as decisões metodológicas.  


---
