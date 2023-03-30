# airbyte-dbt-airflow-bigquery-superset
Repositório para armazenar os artefatos do Pipeline Moderno com AirByte + DBT + Airflow + Big Query + Superset

GCP
BIGQUery
DBT

- Criar conta na Google Cloud
- Criar Projeto na Google Cloud (project id)
- Criar Dataset no Bigquery (dataset id)
- Criar as credenciais no API do Google cloud
- Criar a Chave e baixar o Json e guardar esse arquivo

- Sobe o ambiente do Pipeline
    $ ./setup.sh

- Copia o conection id do airbyte no terminal pra terminar a instalacao do ambiente e criar a dag no airflow

- Entra no Airbyte na porta 8000
- Seta a conexao com a Google planilha usando as credenciais e o id da planilha
- Seta a conexao com o Big Query usando as credenciais e o id do projeto e o id do dataset
- Sync Manual e Overwrite dos dados 
- Configura ou altera a Transfomation apontando pro github do dbt (https://github.com/giu-ferreira-cientista/transformations)
- Volta no airflow e da =star na dag trigger_airbyte_dbt_job
- Checa no Airbytew se ta rodando a Sync
- Checa no BigQuery se subiu o dataset corretamente (tabela transaction-transformed)

* Dataset pronto pra equipe de ML criar o modelo

