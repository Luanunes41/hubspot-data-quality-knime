# HubSpot Data Quality with KNIME

Pipeline de tratamento e padronização de dados para importação de contatos no HubSpot utilizando KNIME.

## Objetivo

Este projeto demonstra a construção de um fluxo de Data Quality voltado para CRM e RevOps, preparando uma base de contatos para importação segura no HubSpot.

## Funcionalidades

* Remoção de espaços em branco
* Padronização de campos de texto
* Validação de e-mails
* Remoção de contatos duplicados
* Normalização de telefones
* Padronização do código do país (+55)
* Criação de indicadores de qualidade dos dados
* Exportação da base tratada

## Fluxo do Processo

CSV Reader

→ Data Cleaning

→ Email Validation

→ Duplicate Removal

→ Phone Normalization

→ Contact Quality Score

→ Export

## Regras Aplicadas

### E-mail

* Conversão para minúsculo
* Validação por expressão regular
* Classificação entre válido e inválido

### Telefone

* Remoção de caracteres especiais
* Padronização para formato internacional
* Inclusão automática do prefixo +55 quando necessário

### Deduplicação

* Identificação de registros duplicados utilizando o e-mail como chave principal

### Qualidade dos Dados

Cálculo de score baseado em:

* E-mail válido
* Telefone preenchido
* Empresa preenchida
* Cargo preenchido

## Tecnologias Utilizadas

* KNIME Analytics Platform
* Git
* GitHub
* HubSpot CRM

## Casos de Uso

* Migração de dados para HubSpot
* Projetos de CRM Ops
* Projetos de RevOps
* Limpeza e enriquecimento de bases de marketing e vendas
* Governança e qualidade de dados

## Estrutura do Projeto

```text
TratamentoBase_HubSpot/
├── workflow.knime
├── data/
├── screenshots/
└── README.md
```

## Próximos Passos

* Tratamento de empresas (Companies)
* Tratamento de negócios (Deals)
* Dashboards de qualidade de dados
* Integração com APIs do HubSpot
* Automação de importações

## Autor

Luan Nunes

Arquiteto de Soluções | HubSpot | RevOps | CRM Ops | Data Quality
