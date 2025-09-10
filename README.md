# Incremental files ingestion from Azure Blob Storage to Microsoft Fabric Lakehouse using PySpark Notebooks  

> This project uses the database provided by the government of Brazil called **Cadastro Geral de Empregados e Desempregados (CAGED)** (General Register of Employed and Unemployed).<br><br>
> This dataset consists of monthly .txt files and is made available on ftp for public download.  <br>  
> Download available at: [ftp://ftp.mtps.gov.br/pdet/microdados/NOVO%20CAGED](ftp://ftp.mtps.gov.br/pdet/microdados/NOVO%20CAGED)  <br> 
> Layout: [ftp://ftp.mtps.gov.br/pdet/microdados/NOVO%20CAGED/Layout%20N%C3%A3o-identificado%20Novo%20Caged%20Movimenta%C3%A7%C3%A3o.xlsx](ftp://ftp.mtps.gov.br/pdet/microdados/NOVO%20CAGED/Layout%20N%C3%A3o-identificado%20Novo%20Caged%20Movimenta%C3%A7%C3%A3o.xlsx)  <br> 


## Shared OneDrive 
Access here: [https://1drv.ms/f/c/34ed68c2d0e7e9fe/EmG9ARE95OlCsLfV-beGVMMB_frLD_fPBHqgvTFStRrOFA?e=amiVXb](https://1drv.ms/f/c/34ed68c2d0e7e9fe/EmG9ARE95OlCsLfV-beGVMMB_frLD_fPBHqgvTFStRrOFA?e=amiVXb)  


## Agenda  

1. Ingerir incrementalmente arquivos Txt do Blob Storage na camada Landing utilizando Microsoft Notebooks PySpark com base na data de modificação;  
2. Carregar para camada bronze (Delta) incrementalmente a partir dos arquivos na Landing zone;  
3. Carregar para camada silver incrementalmente a partir da camada Bronze (Curada);  
4. Carregar para camada gold dados sumarizados e criação do modelo estrela para alimentação de modelo Direct Lake;  
5. Criar um notebook de orquestração sequencial dos outros notebooks (DAG's);  
6. Automatizar processo de detecção de alterações na base para iniciar o processo.  