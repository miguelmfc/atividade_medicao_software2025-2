# Entrega 4 — População, Sujeitos e Amostragem; Instrumentação; Protocolo Operacional; Plano de Análise



## População, sujeitos e amostragem

A população-alvo deste estudo consiste nos usuários de aplicativos de transporte público que publicaram avaliações sobre sua experiência na Google Play Store. Essas avaliações são provenientes de pessoas que utilizaram aplicativos como Moovit, Cittamobi e BHBus, e que registraram suas percepções sobre o funcionamento, a eficiência e a usabilidade desses serviços.
A estratégia de amostragem adotada será não probabilística, uma vez que o estudo se baseia em dados públicos disponíveis na Play Store durante o período de coleta. Todas as avaliações disponíveis nos últimos doze meses serão extraídas e consideradas elegíveis. A escolha desse tipo de amostragem se justifica pelo grande volume de avaliações, pela facilidade de acesso e pela relevância das informações fornecidas pelos usuários.
## Instrumentação e protocolo operacional

A coleta dos dados será realizada por meio de ferramentas de mineração específicas para a Google Play Store. Entre essas ferramentas estão bibliotecas como *google-play-scraper*. Após a coleta, os dados serão armazenados em arquivos CSV para facilitar o uso, a limpeza e o pré-processamento.

O processo de preparação do texto envolve a remoção de elementos não desejados, como emojis, URLs e duplicidades. Em seguida, serão realizadas etapas de tokenização e lematização, que permitirão organizar e padronizar os termos para análises posteriores. A partir desse ponto, técnicas de processamento de linguagem natural serão aplicadas para identificar o sentimento predominante de cada avaliação, classificando-as como positivas, negativas ou neutras. Além disso, o estudo utilizará métodos de categorização temática para agrupar as avaliações em áreas relevantes da usabilidade, tais como navegação, desempenho, confiabilidade, precisão das rotas e qualidade da interface.

Após essas etapas, os dados serão organizados para que diferentes métricas possam ser geradas. Entre essas métricas estão as médias das notas dadas pelos usuários, a proporção de sentimentos em cada cidade e a frequência com que cada categoria de problema é mencionada. Esses resultados permitirão identificar padrões e diferenças entre São Paulo, Belo Horizonte e Rio de Janeiro, considerando tanto os aspectos subjetivos relatados pelos usuários quanto indicadores objetivos extraídos dos metadados.

## Fluxograma

1. Coleta da população

2. Seleção dos sujeitos

3. Mineração das avaliações (Play Store)

4. Limpeza e pré-processamento

5. Classificação dos textos (sentimento / tópicos)

6. Codificação das métricas

7. Análise estatística e comparativa

8. Interpretação dos resultados

9. Conclusões sobre usabilidade
