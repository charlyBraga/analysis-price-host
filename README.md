##Análise de dados, resposta de questãoes de negócios e aplicação de modelos preditivos relacionado à base de dados de anúncios de hospedagem

###Esse projeto visa fazer uma análise exploratória de uma base de dados com anúncios de hospegens, onde o preço se relaciona com outras variáveis,
como local e reviews de usuários. Além disso se tem objetivo de responder questão de negócios, que estão disponíveil no próprio arquivo jupyter notebook. Tudo foi desenvolvido no google colab na linguagem python. Modelos de machine learning como CatBoostRegressor foi utilizado.
Abaixo há mais informações sobre o projeto.

Autor: Charly Braga Ventura
Data de implementação: fevereiro de 2024

####Instruções:
* Independente de qual parte do algoritmo for utilizada, execute o código logo abaixo para importar as bibliotecas.
* O módulo catboost deve ser instalado, caso não esteja.

####Arquivos:
* Relatórico de análise e implementação do projeto: LH_DS_CharlyBraga.ipynb
* Base de dados: este_indicium_precificacao.csv
* O modelo de dados treinado e salvo (model_price_catboost.pkl)  não foi possível salvar aqui no Github, devido ao tamanho. assim salvei ele no google drive e estou disponibilizando o link aqui: https://drive.google.com/file/d/1DnkvOEMKS6c7yOJeyucazbiF_t-QctoU/view?usp=sharing
  

####Dicionário de dados:
*  **id**: Atua como uma chave exclusiva para cada anúncio nos dados do aplicativo
*  **nome**: Representa o nome do anúncio
*  **host_id**: Representa o id do usuário que hospedou o anúncio
*  **host_name**: Contém o nome do usuário que hospedou o anúncio
*  **bairro_group**: Contém o nome do bairro onde o anúncio está localizado
*  **bairro**:Contém o nome da área onde o anúncio está localizado
*  **latitude**: Contém a latitude do local
*  **longitude**: Contém a longitude do local
*  **room_type**: Contém o tipo de espaço de cada anúncio
*  **price**: Contém o preço por noite em dólares listado pelo anfitrião
*  **minimo_noites**: Contém o número mínimo de noites que o usuário deve reservar
*  **numero_de_reviews**: Contém o número de comentários dados a cada listagem
*  **ultima_review**: Contém a data da última revisão dada à listagem
*  **reviews_por_mes**: Contém o número de avaliações fornecidas por mês
*  **calculado_host_listings_count**: Contém a quantidade de listagem por host
*  **disponibilidade_365**: Contém o número de dias em que o anúncio está disponível para reserva

####Alguns metadados da base de dados:
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


