# ⚡Engenharia de Dados: Consumo de Energia Elétrica no Brasil

Este é um projeto **real** de Engenharia de Dados, desenvolvido de ponta a ponta, com o objetivo de praticar e demonstrar todas as etapas do ciclo de vida de dados — desde a coleta até a visualização e integração com um agente de IA para consulta inteligente. Tudo isso utilizando **tecnologias gratuitas e acessíveis**.

---

## 🎯 Objetivo

Construir um pipeline completo de dados sobre o **consumo de energia elétrica no Brasil**, utilizando fontes públicas e ferramentas gratuitas, com foco em:

- Coleta automatizada de dados reais
- Armazenamento bruto e estruturado
- Processamento, transformação e limpeza (ETL)
- Armazenamento em banco de dados relacional
- Criação de um dashboard interativo
- Integração com um agente de IA para análise via linguagem natural

---

## 🧱 Arquitetura do Projeto

```mermaid
graph TD;
    A[Coleta de Dados (ONS)] --> B[Data Lake (CSV/Parquet)]
    B --> C[ETL (Python + Pandas)]
    C --> D[Data Warehouse (PostgreSQL)]
    D --> E[Dashboard (Streamlit)]
    D --> F[AI Agent (LangChain + GPT)]
```

---

## 📚 Tecnologias, Organização e Funcionalidades

Este projeto foi pensado para ser simples, realista e gratuito. Abaixo estão as tecnologias utilizadas, a estrutura do repositório e as funcionalidades implementadas.

### 🛠️ Tecnologias Utilizadas

| Etapa                   | Ferramenta/Ferramentas                     |
|------------------------|--------------------------------------------|
| Coleta de Dados        | Python, requests, pandas                   |
| Armazenamento Bruto    | CSV/Parquet ou MinIO (opcional)            |
| Processamento (ETL)    | Python, pandas                             |
| Banco de Dados         | PostgreSQL (usando Neon, gratuito)         |
| Visualização           | Streamlit                                  |
| Orquestração           | GitHub Actions                             |
| Agente de IA           | LangChain + OpenAI API (plano gratuito)    |
| Variáveis Sensíveis    | python-dotenv                              |
| Versionamento          | Git, GitHub                                |

### 📦 Organização do Repositório

```bash
consumo-energia-brasil/
├── data/
│   ├── raw/             # Dados brutos coletados
│   └── processed/       # Dados transformados
├── etl/
│   └── transform.py     # Script de limpeza e transformação
├── db/
│   └── schema.sql       # Estrutura do banco de dados
├── dashboard/
│   └── app.py           # Código do dashboard em Streamlit
├── ai_agent/
│   └── agent.py         # Agente de IA para consultas aos dados
├── .github/workflows/
│   └── etl.yml          # Automação com GitHub Actions
├── requirements.txt     # Dependências do projeto
└── README.md            # Documentação geral do projeto
```

### 🧠 Funcionalidades do AI Agent

Este projeto contará com um agente de IA capaz de interpretar e responder perguntas sobre os dados de consumo de energia em **linguagem natural**.

#### Exemplos de perguntas:
- "Qual foi o estado com maior consumo residencial em 2023?"
- "Me mostre a média mensal da região Nordeste nos últimos 5 anos."
- "Qual região mais consumiu energia elétrica no verão?"
- "Como foi a evolução do consumo no Brasil entre 2010 e 2024?"

Tecnologias:
- `LangChain`
- `OpenAI GPT`
- Integração com o banco de dados PostgreSQL

---

## 🔗 Fontes de Dados

- [ONS - Operador Nacional do Sistema Elétrico](https://dados.ons.org.br)
- [ANEEL - Agência Nacional de Energia Elétrica](https://dadosabertos.aneel.gov.br)

---

## 🚧 Em Desenvolvimento

- [x] Criação da estrutura do projeto
- [x] Criação do arquivo `requirements.txt`
- [x] Criação e publicação do `README.md`
- [ ] Coleta automatizada dos dados via script
- [ ] Armazenamento em `data/raw/`
- [ ] Criação do ETL
- [ ] Upload dos dados para banco PostgreSQL
- [ ] Construção do dashboard (Streamlit)
- [ ] Integração do AI Agent

---

## 📄 Licença

Este projeto é de uso livre para fins educacionais e profissionais. Sinta-se à vontade para clonar, adaptar ou contribuir.

---

## 👨‍💻 Sobre o Autor

Este projeto está sendo desenvolvido por **um estudante de Engenharia Elétrica em transição para Engenharia de Dados**, com foco total em aplicar os conhecimentos aprendidos na prática, demonstrar domínio técnico e gerar visibilidade profissional para o mercado de tecnologia.

**Conecte-se comigo no [LinkedIn](https://www.linkedin.com/in/matheussmends/).**
