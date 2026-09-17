<div align="center">
  <h2>Logistics & Supply Chain Intelligence 📦</h2>
  <p>Aplicando Engenharia de Dados e Analytics para resolver problemas reais de intralogística, transportes e last-mile.</p>

  <!-- Badges com cores profissionais -->
  <img src="https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=Databricks&logoColor=white" alt="Databricks" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apache-spark&logoColor=white" alt="Spark" />
  <img src="https://img.shields.io/badge/SQL-003B57?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL" />
  <img src="https://img.shields.io/badge/Data_Engineering-2b3137?style=for-the-badge" alt="Data Engineering" />
</div>

<br>

### 📌 Visão Geral do Projeto
Este repositório consolida uma série de análises e pipelines de dados focados no setor de **Logística e Supply Chain**. O objetivo de cada notebook é demonstrar como a transição de dados brutos e ruidosos para métricas de inteligência de mercado pode evitar o vazamento de receitas (*Revenue Leakage*) e otimizar gargalos operacionais.

Todos os projetos foram desenvolvidos no ambiente **Databricks**, utilizando o conceito de **Lakehouse (Arquitetura Medalhão)** para garantir a governança e a qualidade da informação:
* **🥉 Camada Bronze:** Ingestão de dados brutos (simulando falhas reais de sensores IoT, erros de digitação humana e sistemas legados).
* **🥈 Camada Prata:** Limpeza, desduplicação e tratamento de outliers utilizando processamento distribuído via **PySpark** e **Python**.
* **🥇 Camada Ouro:** Aplicação de regras de negócio, agregações e modelagem utilizando **Spark SQL** para consumo de executivos e painéis de BI.

---

### 📊 Portfólio de Análises Logísticas

Abaixo estão os projetos já desenvolvidos e documentados neste repositório. *(Novos projetos e estudos de caso são adicionados continuamente).*

#### 1. Auditoria Financeira de Faturas de Frete (Freight Audit)
* **Problema:** Divergências entre o tarifário contratado e faturas cobradas com erros de cubagem e moedas misturadas.
* **Solução:** Desenvolvimento de um motor de cálculo de peso taxável e padronização cambial.
* **Impacto:** Identificação automatizada de cobranças indevidas, permitindo a recuperação financeira direta.

#### 2. Monitoramento IoT da Cadeia do Frio (Cold Chain)
* **Problema:** Sensores de temperatura de caminhões frigoríficos gerando picos falsos e invalidando cargas perfeitas no sistema.
* **Solução:** Aplicação de *Rolling Averages* (médias móveis) via PySpark em janelas de tempo para limpar o ruído do hardware.
* **Impacto:** Redução drástica de "falsos positivos" de quebra de SLA sanitário, garantindo a integridade dos lotes de vacinas/carnes.

#### 3. Desempenho de Inbound/Outbound no Armazém (WMS)
* **Problema:** Scanners com defeito registrando "cliques duplos", inflando artificialmente o UPH (Units Per Hour) dos operadores.
* **Solução:** Utilização de funções de janela (*Window Functions*) no Spark para desduplicação temporal em milissegundos.
* **Impacto:** Visão real e justa da produtividade, separando gargalos sistêmicos de necessidades reais de retreinamento da equipe.

#### 4. Análise de SLAs e Last-Mile no E-commerce
* **Problema:** Status textuais caóticos preenchidos por motoristas e divergência de fusos horários nos timestamps de entrega.
* **Solução:** Padronização de strings com Expressões Regulares (Regex) e modelagem relacional de tempo de trânsito.
* **Impacto:** Mapeamento em mapa de calor (barras) indicando exatas regiões/estados onde os parceiros de transporte quebram o SLA contratual.

---

### 🛠️ Stack Tecnológica
* **Ambiente de Desenvolvimento:** Databricks Community Edition
* **Linguagens:** Python 3, ANSI SQL, Regex
* **Bibliotecas Principais:** `pyspark.sql`, `pandas`, `numpy`, `datetime`
* **Conceitos Aplicados:** Medallion Architecture, ETL/ELT, Window Functions, Data Cleansing, Imputação de Nulos, Analytics Engineering.

---

### 🚀 Como visualizar os projetos
Os projetos estão armazenados no formato `.html` (exportados diretamente do Databricks) e `.py`/`.ipynb`. 
Para a melhor experiência de leitura, recomendo abrir os arquivos exportados ou visualizar os notebooks diretamente pela interface nativa do GitHub, onde toda a narrativa gerencial (Markdown) e os gráficos estão renderizados.

<br>

<div align="center">
  <i>Desenvolvido para conectar Engenharia de Dados a Resultados de Negócio.</i>
</div>
