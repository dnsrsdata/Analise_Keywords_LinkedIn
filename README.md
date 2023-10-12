# Analise Key Words LinkedIn

## Instruções para execução do projeto

A versão do Python utilizada foi a 3.10.12.

Para rodar o projeto localmente, siga as instruções abaixo:

1. Clone o repositório

```sh
git clone https://github.com/dnsrsdata/Analise_Key_Words_LinkedIn
```

2. Instale as dependências

```sh
pip install -r requirements.txt
```

**Atenção:** Caso você rode os notebooks novamente, é provável que você obtenha
resultados diferentes dos que estão no repositório. Isso ocorre porque os dados
são coletados diretamente do LinkedIn e, portanto, estão sujeitos a alterações.

Outro ponto que vale ressaltar, é que foi possível notar que a disposição dos
elementos na página do LinkedIn pode mudar conforme você acessa a página. Isso
pode fazer com que o código não funcione corretamente. Caso isso ocorra, basta
executar novamente.

## Motivação

Arrumar o LinkedIn é uma tarefa que exige tempo e dedicação. Um dos pontos que
servem como primeira impressão após a busca pelo nome do candidato é o header.
Nesse projeto, vamos analisar os headers de alguns perfis e comparar com as 
palavras chave encontradas nas descrições das vagas.

## Descrição dos arquivos

    - data
        |- created_from_raw
        | |- descriptions_jobs_analista.csv  # dados tratados referente as vagas de analista de dados
        | |- descriptions_jobs_cientista.csv  # dados tratados referente as vagas de cientista de dados 
        | |- headers_analista.csv  # dados tratados referente aos headers de analistas de dados
        | |- headers_cientista.csv  # dados tratados referente aos headers de cientistas de dados
        |- raw
        | |- data_description.txt  # arquivo contendo breves descrições dos arquivos
        | |- descriptions_vaga_Analista.parquet  # dados coletados referente as vagas de analista de dados
        | |- descriptions_vaga_cientista.parquet  # dados coletados referente as vagas de cientista de dados
        | |- headers_Analista.parquet  # dados coletados referente aos headers de analistas de dados
        | |- headers_Cientista.parquet  # dados coletados referente aos headers de cientistas de dados
        |
        - notebooks
        |- data_modelling.ipynb # Notebook onde os dados foram tratados  
        |- scrapper.ipynb # Notebook onde os dados foram coletados 
        |
        - README.md  # Arquivo contendo as informações do projeto
        - requirements.txt # Arquivo contendo os pacotes necessários para reproduzir o projeto

## Resultado

Os painéis gerados a partir dos dados coletados podem ser conferidos na pasta **paineis**.