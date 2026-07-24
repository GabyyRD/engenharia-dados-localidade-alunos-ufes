# Engenharia de Dados - Localidade dos Alunos UFES

## 📌 Objetivo do Projeto

Este projeto tem como objetivo desenvolver um pipeline de Engenharia de Dados utilizando informações de localidade dos alunos da Universidade Federal do Espírito Santo (UFES).

A partir de um arquivo CSV contendo dados de matrícula, curso, município e estado dos estudantes, foi construído um fluxo completo de dados utilizando a arquitetura em camadas **Bronze, Silver e Gold**, seguindo boas práticas utilizadas em ambientes profissionais de Engenharia de Dados.

O projeto realiza a ingestão, tratamento, padronização e transformação dos dados, disponibilizando informações estruturadas para análises sobre distribuição geográfica dos alunos, cursos e evolução dos ingressantes ao longo dos anos.

Apesar de ser uma base de dados muito pequena (cerca de 2000 alunos), o objetivo é aprender as ferramentas com uma base pequena para eu conseguir validar se estava fazendo corretamente e com uma base real de dados onde atuo como bolsista.

---

## 🏗 Arquitetura do Projeto

O pipeline foi desenvolvido utilizando o conceito de **Medallion Architecture**, uma arquitetura amplamente utilizada em plataformas de dados modernas.

A organização das camadas é:Dados Brutos (CSV) -> Bronze Layer -> Silver Layer -> Gold Layer -> Análises


Cada camada possui uma responsabilidade específica:

### 🥉 Bronze

Responsável pela ingestão dos dados originais, mantendo uma cópia estruturada do arquivo de origem.

### 🥈 Silver

Responsável pela limpeza e preparação dos dados, incluindo:

### 🥇 Gold

Responsável pela criação das tabelas analíticas utilizadas para responder perguntas de negócio.

---

