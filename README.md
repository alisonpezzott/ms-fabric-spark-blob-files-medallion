# Incremental files ingestion from Azure Blob Storage to Microsoft Fabric Lakehouse using PySpark Notebooks  

> This project uses the database provided by the government of Brazil called **Cadastro Geral de Empregados e Desempregados (CAGED)** (General Register of Employed and Unemployed).<br><br>
> This dataset consists of monthly .txt files and is made available on ftp for public download.  <br>  
> Download available at: [ftp://ftp.mtps.gov.br/pdet/microdados/NOVO%20CAGED](ftp://ftp.mtps.gov.br/pdet/microdados/NOVO%20CAGED)  <br> 
> Layout: [ftp://ftp.mtps.gov.br/pdet/microdados/NOVO%20CAGED/Layout%20N%C3%A3o-identificado%20Novo%20Caged%20Movimenta%C3%A7%C3%A3o.xlsx](ftp://ftp.mtps.gov.br/pdet/microdados/NOVO%20CAGED/Layout%20N%C3%A3o-identificado%20Novo%20Caged%20Movimenta%C3%A7%C3%A3o.xlsx)  <br> 


## Shared OneDrive 
Access here: [https://1drv.ms/f/c/34ed68c2d0e7e9fe/EmG9ARE95OlCsLfV-beGVMMB_frLD_fPBHqgvTFStRrOFA?e=amiVXb](https://1drv.ms/f/c/34ed68c2d0e7e9fe/EmG9ARE95OlCsLfV-beGVMMB_frLD_fPBHqgvTFStRrOFA?e=amiVXb)  


## Agenda  

1. Blob Storage -> Landing (Files);
2. Landing -> Bronze (As-is);  
3. Bronze -> Silver (Curated);  
4. Silver -> Gold (Agg) + BI;  
5. DAG;  
6. Automatize date modification detect.
   