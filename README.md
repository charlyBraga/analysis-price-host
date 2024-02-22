
Autor: Charly Braga Ventura
Data de implementação: fevereiro de 2024

Instruções:
* Independente de qual parte do algoritmo for utilizada, execute o código logo abaixo para importar as bibliotecas.
* O módulo catboost deve ser instalado, caso não esteja.


Dicionário de dados:
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

Metadados baseado no dataFrame do python:
Quantidade de linhas (registros): 48.894
Quantidade de colunas (variáveis): 16
 #   Coluna                         Qtd não nulos   Tipo 
---  ------                         --------------  -----  
 0   id                             48894 non-null  int64  
 1   nome                           48878 non-null  object 
 2   host_id                        48894 non-null  int64  
 3   host_name                      48873 non-null  object 
 4   bairro_group                   48894 non-null  object 
 5   bairro                         48894 non-null  object 
 6   latitude                       48894 non-null  float64
 7   longitude                      48894 non-null  float64
 8   room_type                      48894 non-null  object 
 9   price                          48894 non-null  int64  
 10  minimo_noites                  48894 non-null  int64  
 11  numero_de_reviews              48894 non-null  int64  
 12  ultima_review                  38842 non-null  object 
 13  reviews_por_mes                38842 non-null  float64
 14  calculado_host_listings_count  48894 non-null  int64  
 15  disponibilidade_365            48894 non-null  int64  
dtypes: float64(3), int64(7), object(6)
memory usage: 6.0+ MB
