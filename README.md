# Dashboard de Análise de Salários na Área de TI 📊🌐

Uma aplicação interativa de alta performance desenvolvida em **Streamlit** para explorar e visualizar dados de mercado sobre os salários na área de tecnologia em escala global.

---

## 📐 Filosofia de Arquitetura

Este projeto foi desenhado sob o princípio de **consumo otimizado de dados**. Para garantir que a aplicação web responda instantaneamente aos filtros do usuário sem gargalos de processamento, todo o trabalho pesado de limpeza e tratamento de dados foi delegado para um pipeline isolado de ETL.

O Dashboard consome de forma assíncrona o arquivo tratado e hospedado dinamicamente:
`Dado-Final.csv` originado a partir do repositório de engenharia de dados.

---

## 📈 Funcionalidades Principais

- **Métricas Gerais Dinâmicas:** Exibição rápida de salário médio, salário máximo, total de registros analisados e cargo de maior frequência.
- **Filtros Interativos:** Painel lateral dinâmico permitindo que o usuário refine a análise em tempo real por diferentes parâmetros.
- **Mapa Coroplético Global:** Visualização espacial interativa utilizando a projeção de mapas do Plotly para exibir o salário médio de Cientistas de Dados agrupados por país (utilizando codificação geográfica ISO-3).
- **Gráficos Avançados:** Gráficos interativos integrados com a biblioteca Plotly que respondem dinamicamente ao estado dos filtros da aplicação.

---

## 🛠️ Tecnologias Utilizadas

- **Python** (Linguagem de desenvolvimento)
- **Streamlit** (Framework para construção de interfaces web interativas)
- **Plotly** (Engine de renderização de gráficos estatísticos e mapas interativos de alta performance)
- **Pandas** (Leitura assíncrona e filtragem ágil dos dados em memória)

---

## 🚀 Como Rodar o Dashboard Localmente

1. Clone o repositório:
   ```bash
   git clone [https://github.com/DandiReis/DashBoard-Salarios-de-TI.git](https://github.com/DandiReis/DashBoard-Salarios-de-TI.git)
   cd DashBoard-Salarios-de-TI
   
2. Crie e ative seu ambiente virtual (recomendado):
   ```Bash    
   python -m venv .venv       
   source .venv/bin/activate
   ```    
   **No Windows use:**
   ```Bash
   .venv\Scripts\activate       
   ```

4. Instale as dependências:
   ```bash
   pip install -r requirements.txt      

5. Execute o aplicativo Streamlit:
   ```Bash     
   streamlit run app.py         
---

## 🔗 Pipeline de Dados Relacionado
O processo de higienização, tradução e estruturação dos dados que abastecem este Dashboard está hospedado no repositório dedicado ao pipeline de dados:
👉 **[Limpeza-Plotagem-Dados](https://github.com/DandiReis/Limpeza-Plotagem-Dados)**
