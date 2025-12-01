# Entrega 4 — População, Sujeitos e Amostragem; Instrumentação; Protocolo Operacional; Plano de Análise

Esta entrega descreve, de forma narrativa, todos os elementos metodológicos necessários para a execução do estudo sobre a usabilidade de aplicativos de transporte público, especificamente nas cidades de São Paulo, Belo Horizonte e Rio de Janeiro. O objetivo é apresentar, de maneira fluida e contínua, a definição da população, o processo de amostragem, os instrumentos utilizados para a coleta e análise dos dados, além do protocolo operacional e do plano de análise que será seguido antes da execução prática.

## População, sujeitos e amostragem

A população-alvo deste estudo consiste nos usuários de aplicativos de transporte público que publicaram avaliações sobre sua experiência na Google Play Store. Essas avaliações são provenientes de pessoas que utilizaram aplicativos como Moovit, Cittamobi e outras plataformas semelhantes, e que registraram espontaneamente suas percepções sobre o funcionamento, a eficiência e a usabilidade desses serviços. Os sujeitos da pesquisa não são os indivíduos de forma direta, mas sim os textos das avaliações que eles disponibilizaram publicamente, os quais representam seus relatos, opiniões e críticas.

A estratégia de amostragem adotada será não probabilística por conveniência, uma vez que o estudo se baseia em dados públicos disponíveis na Play Store durante o período de coleta. Assim, todas as avaliações disponíveis nos últimos doze meses serão extraídas e consideradas elegíveis. A escolha desse tipo de amostragem se justifica pelo grande volume de avaliações, pela facilidade de acesso e pela relevância das informações fornecidas pelos usuários. Estima-se que o conjunto final conterá entre dois mil e dez mil comentários, dependendo da quantidade de avaliações armazenadas pelos aplicativos-alvo no recorte temporal definido.

## Instrumentação e protocolo operacional

A coleta dos dados será realizada por meio de ferramentas de mineração específicas para a Google Play Store. Entre essas ferramentas estão bibliotecas como *google-play-scraper*, scripts próprios desenvolvidos em Python utilizando *Requests* ou *Selenium*, e outros recursos semelhantes destinados à extração automatizada de texto, nota, data, versão do aplicativo e demais metadados das avaliações. Após a coleta, os dados serão armazenados em arquivos CSV ou JSON para facilitar o manejo, a limpeza e o pré-processamento.

O processo de preparação do texto envolve a remoção de elementos indesejados, como stopwords, emojis, URLs, duplicidades e erros típicos de escrita. Em seguida, serão realizadas etapas de tokenização e lematização, que permitirão organizar e padronizar os termos para análises posteriores. A partir desse ponto, técnicas de processamento de linguagem natural serão aplicadas para identificar o sentimento predominante de cada avaliação, classificando-as como positivas, negativas ou neutras. Além disso, o estudo utilizará métodos de categorização temática para agrupar as avaliações em áreas relevantes da usabilidade, tais como navegação, desempenho, confiabilidade, precisão das rotas e qualidade da interface.

Após essas etapas, os dados serão organizados para que diferentes métricas possam ser geradas. Entre essas métricas estão as médias das notas dadas pelos usuários, a proporção de sentimentos em cada cidade e a frequência com que cada categoria de problema é mencionada. Esses resultados permitirão identificar padrões e diferenças entre São Paulo, Belo Horizonte e Rio de Janeiro, considerando tanto os aspectos subjetivos relatados pelos usuários quanto indicadores objetivos extraídos dos metadados.

## Fluxograma do processo 

```mermaid
flowchart TD

A[Definição do Escopo<br>(Apps e Cidades)] --> B[Mineração de Dados<br>Scraper Google Play]
B --> C[Armazenamento dos Dados<br>(CSV/JSON)]
C --> D[Limpeza e Pré-processamento<br>(Stopwords, Lematização)]
D --> E[Análise de Sentimento<br>(Modelo NLP)]
E --> F[Classificação Temática<br>(Categorias de Usabilidade)]
F --> G[Geração de Métricas<br>(Médias, Frequências, Tendências)]
G --> H[Comparação Entre Cidades<br>(SP, BH, RJ)]
H --> I[Interpretação dos Resultados<br>à luz da literatura UX]
I --> J[Preparação do Relatório Final]
