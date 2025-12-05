5.1 Ameaças à Validade Interna
Ameaças à validade interna referem-se a fatores que podem comprometer a atribuição causal ou a interpretação de diferenças observadas entre os grupos comparados.

A5.1.1 Viés de Seleção da Fonte de Dados (Ameaça de Amostragem)
Descrição: Os dados são provenientes exclusivamente de avaliações públicas da Google Play Store. Usuários que publicam avaliações online podem constituir um subgrupo não representativo da população total de usuários, tendendo a ser aqueles com experiências extremamente positivas ou negativas.

Categoria: Viés de seleção/amostragem.

Estratégias de Mitigação:

Transparência Analítica: Reconhecer explicitamente esta limitação nas conclusões do estudo, qualificando os resultados como representativos da "população de avaliadores", não de todos os usuários.

Análise de Padrões de Envolvimento: Investigar, dentro dos metadados disponíveis, se há padrões que indiquem vieses sistemáticos (ex.: picos de avaliações negativas após atualizações).

Contextualização com Literatura: Comparar os perfis de sentimento e tópicos encontrados com estudos que utilizaram outros métodos (como surveys) para identificar possíveis desvios.

A5.1.2 História e Maturidade (Ameaças Temporais)
Descrição: Mudanças nos aplicativos (atualizações de versão, correções de bugs) ou no contexto do sistema de transporte das cidades (mudanças de linhas, greves) durante o período de coleta podem afetar as avaliações, confundindo comparações entre períodos ou grupos.

Categoria: Confundimento temporal.

Estratégias de Mitigação:

Controle por Versão: Incluir a versão do aplicativo como metadado na coleta e realizar análises segmentadas para períodos de versões estáveis.

Registro de Eventos Externos: Documentar eventos conhecidos (grandes atualizações, mudanças significativas no transporte público) que possam ter impactado as percepções dos usuários.

Análise de Sazonalidade: Verificar a distribuição das avaliações ao longo do tempo para identificar tendências ou pontos de inflexão não aleatórios.

A5.1.3 Instrumentação (Variação no Processo de Medida)
Descrição: Alterações no algoritmo de análise de sentimento (PLN) ou nos critérios de categorização temática durante o processamento dos dados podem introduzir variação não atribuível aos aplicativos ou cidades.

Categoria: Viés de medição/instrumentação.

Estratégias de Mitigação:

Protocolo Operacional Fixo: Definir e documentar de forma precisa todos os parâmetros, modelos e dicionários de termos a serem utilizados na análise de PLN e categorização antes do início do processamento.

Validação e Consistência: Aplicar o protocolo completo a um subconjunto de dados de controle em diferentes momentos para verificar a consistência dos resultados.

5.2 Ameaças à Validade Externa
Ameaças à validade externa referem-se à capacidade de generalizar os resultados do estudo para outros contextos, populações ou momentos.

A5.2.1 Amostragem Não Probabilística e Especificidade do Contexto
Descrição: A amostra é composta por todos os dados disponíveis para três aplicativos específicos em três capitais brasileiras durante um período determinado. Isso limita a generalização para outras cidades (com sistemas de transporte diferentes), outros aplicativos, usuários de outras plataformas (ex.: iOS) ou períodos futuros.

Categoria: Validade de população e ecológica.

Estratégias de Mitigação:

Delimitação Clara do Universo: Definir e comunicar precisamente o universo da pesquisa: "usuários dos aplicativos X, Y e Z que publicaram avaliações na Google Play Store para as cidades A, B e C no período P".

Descrição Rica do Contexto: Fornecer uma descrição detalhada das características dos aplicativos e do contexto urbano das três cidades, permitindo que outros pesquisadores avaliem a transferibilidade dos achados para contextos semelhantes.

Estrutura Metodológica Replicável: Documentar a metodologia de forma que possa ser aplicada a outros conjuntos de apps e cidades, promovendo estudos comparativos futuros que possam ampliar a generalização.

5.3 Ameaças à Validade de Construto
Ameaças à validade de construto referem-se ao grau em que os procedimentos de medição representam adequadamente os conceitos teóricos em estudo (ex.: "usabilidade", "satisfação").

A5.3.1 Operacionalização Incompleta de "Usabilidade"
Descrição: O estudo opera com o construto de "usabilidade percebida" a partir de avaliações espontâneas. A norma ISO 9241-11 define usabilidade através de três dimensões (eficiência, eficácia e satisfação), que podem não ser cobertas de forma completa ou equilibrada nos comentários dos usuários, que tendem a focar em problemas pontuais ou aspectos emocionais.

Categoria: Validade de medição (viés do construto).

Estratégias de Mitigação:

Framework de Mapeamento Teórico-Pragmático: Desenvolver uma matriz de categorização que relacione explicitamente os tópicos e termos extraídos dos comentários com as dimensões da usabilidade e atributos de qualidade de software (ex.: confiabilidade, desempenho).

Validação por Especialistas: Submeter a matriz de categorização e uma amostra de comentários classificados à avaliação de especialistas em Interação Humano-Computador (IHC) ou Experiência do Usuário (UX) para verificar a adequação da operacionalização.

Análise Multimétrica: Complementar a análise textual com métricas objetivas derivadas dos dados (ex.: correlação entre sentimento e nota, M4.1), criando uma visão mais robusta do construto.

A5.3.2 Limitações do Processamento de Linguagem Natural (PLN)
Descrição: Os algoritmos de análise de sentimentos e tópicos podem falhar em capturar nuances de linguagem como ironia, sarcasmo, dupla negação ou contextos culturais e regionais específicos, levando a classificações errôneas.

Categoria: Viés de instrumento/ferramenta.

Estratégias de Mitigação:

Validação Manual de Subamostra: Classificar manualmente uma subamostra aleatória e estratificada dos comentários (ex.: 10-15%) e comparar os resultados com a classificação automatizada para calcular e reportar uma métrica de acurácia/concordância (ex.: Coeficiente Kappa).

Ajuste e Contextualização do Modelo: Utilizar ou fine-tunar modelos de PLN treinados em português brasileiro e, se possível, em domínios similares. Criar e utilizar um dicionário de termos e gírias regionais relacionadas ao transporte nas cidades em estudo.

Análise de Consistência Cruzada: Verificar a consistência lógica entre a classificação de sentimento (positivo/negativo) e a nota numérica atribuída (1-5 estrelas) para identificar possíveis falhas grosseiras na classificação automatizada.

5.4 Ameaças à Validade Estatística e de Conclusão
Ameaças à validade estatística referem-se à adequação dos testes e procedimentos estatísticos. Ameaças à validade de conclusão referem-se a erros na inferência sobre a relação entre tratamento e resultado.

A5.4.1 Poder Estatístico Desbalanceado
Descrição: O volume de avaliações (tamanho da amostra) varia significativamente entre os diferentes aplicativos e, possivelmente, entre as cidades (ex.: Moovit tem avaliações globais, BHBus é local). Amostras muito desiguais podem reduzir o poder estatístico para detectar diferenças em grupos menores ou levar a violações de pressupostos em testes paramétricos.

Categoria: Poder do teste / Pressupostos estatísticos.

Estratégias de Mitigação:

Escolha Adequada de Testes: Priorizar o uso de testes estatísticos não paramétricos (ex.: Teste de Kruskal-Wallis, Teste U de Mann-Whitney) para comparações de grupos, pois são menos sensíveis a tamanhos amostrais desiguais e não exigem normalidade estrita.

Análise de Sensibilidade: Realizar análises com diferentes subamostras ou técnicas de bootstrapping para verificar a robustez dos resultados encontrados.

Reporte de Intervalos de Confiança: Sempre que possível, reportar medidas de efeito acompanhadas de seus intervalos de confiança, em vez de apenas valores-p, fornecendo uma noção da precisão e variabilidade da estimativa.

A5.4.2 Inferência Causal Inadequada (Natureza Observacional)
Descrição: O desenho do estudo é observacional e comparativo, não experimental. Ele identifica associações e padrões, mas não pode estabelecer relações de causa e efeito definitivas. Por exemplo, encontrar mais queixas sobre interface em um app não prova que a interface causa a insatisfação; pode haver um fator de confusão não observado.

Categoria: Validade de conclusão (inferência causal).

Estratégias de Mitigação:

Linguagem Precisa e Cautelosa: Em toda a redação do estudo, utilizar termos como "associado a", "relacionado com", "correlacionado", "pode sugerir", e evitar termos causais como "causa", "leva a", "resulta em", a menos que haja forte suporte teórico e controle de variáveis.

Discussão de Fatores de Confusão: Na seção de discussão, identificar e debater possíveis variáveis de confusão (ex.: expectativas do usuário, qualidade objetiva do transporte na cidade) que poderiam explicar as associações observadas.

Enquadramento como Estudo Exploratório/Descritivo: Posicionar claramente o trabalho como uma análise descritiva e comparativa que gera hipóteses e insights, e não como um teste causal definitivo.

A5.4.3 Viés do Pesquisador na Análise e Interpretação
Descrição: Existe o risco de que expectativas prévias (como as hipóteses H1-H4) influenciem inconscientemente a maneira como os dados são processados, analisados ou interpretados, levando a um viés de confirmação.

Categoria: Viés cognitivo / Validade de conclusão.

Estratégias de Mitigação:

Análise Exploratória Independente: Realizar uma fase inicial de análise exploratória de dados (AED) sem o objetivo direto de testar as hipóteses, para identificar padrões inesperados.

Documentação Auditável: Manter um registro detalhado (log analítico) de todas as decisões tomadas durante o processamento, limpeza, categorização e análise dos dados, justificando cada escolha metodológica.

Revisão por Pares ou Supervisor: Submeter os planos de análise e os resultados preliminares à revisão de colegas ou do orientador para obtenção de feedback e desafio das interpretações.

