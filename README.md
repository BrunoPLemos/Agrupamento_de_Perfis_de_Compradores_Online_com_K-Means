Este projeto realiza uma análise de segmentação de visitantes de um site de comércio eletrônico utilizando o algoritmo de K-Means Clustering. O objetivo é identificar padrões de comportamento dos usuários que podem ajudar a prever a propensão de conversão (Revenue).

Tecnologias e Bibliotecas Utilizadas
Python 
Pandas
NumPy
Matplotlib
Seaborn
scikit-learn

1. Carregamento e Pré-processamento dos Dados
Leitura de um dataset com dados de sessões de usuários em um e-commerce.

Seleção das 6 primeiras variáveis numéricas.

Aplicação de padronização (StandardScaler) para normalizar os dados.

2. Definição do Número de Clusters
Aplicação do Método do Cotovelo, avaliando a soma das variâncias internas (inertia).

Cálculo do Coeficiente de Silhueta, que mede a qualidade da separação dos clusters.

3. Treinamento com KMeans
Treinamento do modelo com k=2 (melhor Silhueta) e k=3 (ponto do cotovelo).

Inclusão dos rótulos de cluster no DataFrame original.

4. Análise dos Grupos
Avaliação das características médias dos usuários em cada grupo.

Comparação dos clusters quanto às variáveis BounceRates e Revenue para identificar possíveis perfis de compradores mais propensos à conversão.

Principais Resultados
k=2 clusters obteve melhor score de Silhueta.

Um dos clusters apresenta maior taxa de conversão (Revenue) e menor BounceRate, indicando um perfil de visitante mais engajado.

O modelo pode ser utilizado para identificar automaticamente perfis de visitantes que tendem mais à compra.

