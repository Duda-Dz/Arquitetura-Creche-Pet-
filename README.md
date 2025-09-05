# 🐾 Creche Pet – Arquitetura em Nuvem com AWS

### Este projeto apresenta a arquitetura de um aplicativo para gestão de uma creche pet, utilizando serviços da AWS.
### A arquitetura foi modelada no draw.io e contempla o fluxo de cadastro de pets e relatórios de comportamento, com foco em boas práticas de escalabilidade, segurança e custo.

## ⚙️Ferramentas Demonstradas: 

![Amazon S3](https://img.shields.io/badge/Amazon%20S3-FF9900?style=for-the-badge&logo=amazons3&logoColor=white) ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white) ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black) ![RDS](https://img.shields.io/badge/Amazon%20RDS-527FFF?style=for-the-badge&logo=amazon-rds&logoColor=white)

## 🚀 Tecnologias e Serviços Utilizados
- Draw.io: Modelagem da Arquitetura
  
- Amazon EC2: Hospedagem e processamento do backend.

- Amazon EBS: Armazenamento persistente temporário para EC2.

- Amazon S3: Armazenamento de fotos, documentos e relatórios.

- Amazon S3 Glacier: Arquivamento de longo prazo para cadastros inativos.

- Amazon API Gateway: Entrada e validação de requisições.

- AWS Lambda: Processamento serverless para validação, automação e redirecionamento de dados.

- Amazon RDS (MySQL): Armazenamento estruturado de dados.

- Amazon SES: Envio de relatórios e notificações por e-mail.

- Amazon QuickSight: Dashboards e visualização analítica dos dados.

  ## 📊 Fluxo Geral da Arquitetura

- Tutor cadastra o pet no aplicativo.

- EC2 (com EBS) processa o cadastro.

- Dados estruturados → armazenados no Amazon RDS.

- Fotos e documentos → armazenados no S3, sendo arquivos antigos movidos para o S3 Glacier.

- Cuidador envia relatórios → processados via EBS, validados por Lambda.

- Relatórios armazenados no S3, disponibilizados via:
-  `Amazon SES: Envio por e-mail`
-  `Amazon QuickSight → Visualização em dashboards.`

## 📌 Objetivo do Projeto

### Este repositório tem como objetivo demonstrar a construção de uma arquitetura em nuvem para um aplicativo real, aplicando os conceitos aprendidos em AWS dentro de um cenário prático.




