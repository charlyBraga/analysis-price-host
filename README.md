## Análise de dados, resposta de questãoes de negócios e aplicação de modelos preditivos relacionado à base de dados de anúncios de hospedagem

### Esse projeto visa fazer uma análise exploratória de uma base de dados com anúncios de hospegens, onde o preço se relaciona com outras variáveis, como local e reviews de usuários. Além disso se tem objetivo de responder questão de negócios, que estão disponíveil no próprio arquivo jupyter notebook. Tudo foi desenvolvido no google colab na linguagem python. Modelos de machine learning como CatBoostRegressor foi utilizado.
Abaixo há mais informações sobre o projeto.

Autor: Charly Braga Ventura

Data de implementação: fevereiro de 2024

#### Instruções:
* Independente de qual parte do algoritmo for utilizada, execute o bloco onde estão as bibliotecas.
* O módulo "catboost" deve ser instalado, caso não esteja.

#### Arquivos presente nesse repositório:
* Relatórico de análise e implementação do projeto: LH_DS_CharlyBraga.ipynb
* Base de dados: este_indicium_precificacao.csv
* O modelo de dados treinado e salvo: model_price_catboost.pkl, não foi possível salvar aqui no Github, devido ao tamanho, assim salvei ele no google drive e estou disponibilizando o link aqui: https://drive.google.com/file/d/1DnkvOEMKS6c7yOJeyucazbiF_t-QctoU/view?usp=sharing
  

#### Dicionário de dados:
O dicionário de dados visa explicar os significados das colunas da base de dados em forma de tabela utilizada neste projeto. 
Cada coluna tem um tipo definido, como exemplo, idade geralmente é repsentada por tipo número inteiro e valor monetário por tipo número decimal.
*  **id**: identificação exclusiva para cada anúncio nos dados do aplicativo, ou seja, cada linha terá um valor único (tipo número inteiro)
*  **nome**: nome do anúncio (tipo texto)
*  **host_id**: identicação do usuário que hospedou o anúncio (tipo número inteiro)
*  **host_name**: nome do usuário que hospedou o anúncio (tipo texto)
*  **bairro_group**: nome do bairro onde o anúncio está localizado (tipo texto)
*  **bairro**: nome da área onde o anúncio está localizado (tipo texto)
*  **latitude**: latitude do local (tipo número decimal)
*  **longitude**: longitude do local (tipo número decimal)
*  **room_type**: tipo de espaço de cada anúncio  (tipo texto)
*  **price**: preço por noite em dólares listado pelo anfitrião (tipo número decimal)
*  **minimo_noites**: número mínimo de noites que o usuário deve reservar (tipo número inteiro)
*  **numero_de_reviews**: número de comentários dados a cada listagem (tipo número inteiro)
*  **ultima_review**: data da última revisão dada à listagem (tipo data)
*  **reviews_por_mes**: número de avaliações fornecidas por mês (tipo número inteiro)
*  **calculado_host_listings_count**: quantidade de listagem por host  (tipo número inteiro)
*  **disponibilidade_365**: número de dias em que o anúncio está disponível para reserva (tipo número inteiro)

#### Alguns metadados da base de dados:
* Quantidade de linhas (registros): 48.894
* Quantidade de colunas (variáveis): 16
  
| #   | Colunas                        | Qtd não nulos | Tipos    |
|-----|--------------------------------|---------------|----------|
| 0   | id                             | 48894 não-nulo| inteiro  |
| 1   | nome                           | 48878 não-nulo| texto    |
| 2   | host_id                        | 48894 não-nulo| inteiro  |
| 3   | host_name                      | 48873 não-nulo| texto    |
| 4   | bairro_group                   | 48894 não-nulo| texto    |
| 5   | bairro                         | 48894 não-nulo| texto    |
| 6   | latitude                       | 48894 não-nulo| decimal  |
| 7   | longitude                      | 48894 não-nulo| decimal  |
| 8   | room_type                      | 48894 não-nulo| texto    |
| 9   | price                          | 48894 não-nulo| inteiro  |
| 10  | minimo_noites                  | 48894 não-nulo| inteiro  |
| 11  | numero_de_reviews              | 48894 não-nulo| inteiro  |
| 12  | ultima_review                  | 38842 não-nulo| texto    |
| 13  | reviews_por_mes                | 38842 não-nulo| decimal  |
| 14  | calculado_host_listings_count  | 48894 não-nulo| inteiro  |
| 15  | disponibilidade_365            | 48894 não-nulo| inteiro  |


