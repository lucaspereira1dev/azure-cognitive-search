# # **Laboratório de Organização e Pesquisa de Documentos com IA**  

**Objetivo**  
Este projeto visa demonstrar a aplicação de técnicas de **Inteligência Artificial (IA)** para ingestão, indexação e exploração de documentos, permitindo a extração eficiente de conhecimento a partir de grandes volumes de dados.  

---

## **Tecnologias e Ferramentas Utilizadas**  
✔ **Azure AI Search** (para indexação e busca inteligente)  
✔ **Azure Cognitive Services** (processamento de linguagem natural - NLP)  
✔ **Python e Jupyter Notebooks** (automação e análise)  
✔ **Armazenamento em Nuvem (Blob Storage)** (para ingestão de documentos)  

---

## **Fluxo de Trabalho**  

### **1. Ingestão de Conteúdo para IA**  
- Coleta de documentos em formatos variados (PDF, TXT, DOCX, etc.).  
- Upload dos arquivos para um **Azure Blob Storage**.  
- Pré-processamento de texto (limpeza, normalização, extração de metadados).  

### **2. Criação de Índices Inteligentes**  
- Configuração de um **Azure AI Search** para indexação semântica.  
- Definição de campos indexados (texto, entidades, palavras-chave).  
- Aplicação de **NLP (Cognitive Services)** para enriquecimento de dados (reconhecimento de entidades, análise de sentimentos).  

### **3. Exploração dos Dados Organizados**  
- Consultas avançadas usando **linguagem natural** (ex: "Encontre documentos sobre gestão escolar de 2023").  
- Visualização de insights via **Dashboards (Power BI opcional)**.  
- Exportação de resultados para análise posterior.  

---

## **Estrutura do Repositório**  
```
.
├── /data/                  # Arquivos brutos para ingestão  
├── /notebooks/             # Jupyter Notebooks de processamento  
│   ├── 01_data_ingestion.ipynb  
│   ├── 02_index_creation.ipynb  
│   └── 03_query_exploration.ipynb  
├── /scripts/               # Scripts Python para automação  
├── /docs/                  # Documentação complementar  
├── README.md               # Este arquivo  
└── requirements.txt        # Dependências do projeto  
```

---

## **Como Executar o Projeto**  

### **Pré-requisitos**  
- Conta no **Microsoft Azure** (com acesso a AI Search e Cognitive Services).  
- Python 3.8+ e bibliotecas listadas em `requirements.txt`.  

### **Passos para Configuração**  
1. Clone o repositório:  
   ```bash
   git clone https://github.com/lucaspereira1dev/organizacao-docs-ia.git
   cd organizacao-docs-ia
   ```  
2. Instale as dependências:  
   ```bash
   pip install -r requirements.txt
   ```  
3. Configure as credenciais do Azure no arquivo `.env`:  
   ```ini
   AZURE_SEARCH_ENDPOINT=seu-endpoint
   AZURE_SEARCH_KEY=sua-chave
   AZURE_STORAGE_CONN_STRING=sua-string-de-conexao
   ```  
4. Execute os notebooks na ordem:  
   - `01_data_ingestion.ipynb` (Ingestão)  
   - `02_index_creation.ipynb` (Indexação)  
   - `03_query_exploration.ipynb` (Consulta)  

---

## **Entregáveis Esperados**  
✅ **Repositório organizado** com código e documentação.  
✅ **Índice de busca funcional** no Azure AI Search.  
✅ **Relatório de insights** extraídos dos documentos (ex: entidades mais frequentes, tópicos dominantes).  
✅ **Exemplos de queries** e resultados obtidos.  

---

## **Referências**  
- [Documentação do Azure AI Search](https://learn.microsoft.com/azure/search/)  
- [Cognitive Services - NLP](https://azure.microsoft.com/products/cognitive-services/language-service/)  

---
