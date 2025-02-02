# 🏡 Análise de Oportunidades no Mercado Imobiliário  

<img src="03-Recursos/imagem_capa.png">


<div align="center">
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white"></a>
  <a href="https://jupyter.org/"><img src="https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter"></a>
  <a href="https://pandas.pydata.org/"><img src="https://img.shields.io/badge/Pandas-2.2.2-green?logo=pandas"></a>
  <a href="https://numpy.org/"><img src="https://img.shields.io/badge/NumPy-1.26.4-blue?logo=numpy"></a>
  <a href="https://matplotlib.org/"><img src="https://img.shields.io/badge/Matplotlib-3.10.0-blue?logo=matplotlib"></a>
  <a href="https://seaborn.pydata.org/"><img src="https://img.shields.io/badge/Seaborn-0.13.2-blue?logo=seaborn"></a>
  <a href="https://scikit-learn.org/"><img src="https://img.shields.io/badge/Scikit--Learn-1.6.1-orange?logo=scikit-learn&logoColor=white"></a>
  <a href="https://geopandas.org/"><img src="https://img.shields.io/badge/GeoPandas-1.0.1-blue?logo=geopandas"></a>
  <a href="https://lightgbm.readthedocs.io/"><img src="https://img.shields.io/badge/LightGBM-4.5.0-green"></a>
  <a href="https://catboost.ai/"><img src="https://img.shields.io/badge/CatBoost-2.0-yellow"></a>
  <a href=""><img src="https://img.shields.io/badge/Status-Completed-green"></a>
  <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>
</div>

---

## 📝 **Descrição do Projeto**  

Neste projeto, analisamos o comportamento de estados brasileiros no setor imobiliário com foco na faixa etária de consumidores predominante (38 a 58 anos). A análise consiste em prever a tendência de crescimento de consumidores e identificar oportunidades futuras por estado.

O projeto foi estruturado em etapas que vão desde a coleta e manipulação de dados até a aplicação de modelos preditivos e a segmentação dos estados por meio de clusterização.

**Objetivos principais:**
- Estimar o comportamento do mercado imobiliário entre 2021 e 2022 com base nos dados históricos de 2007 a 2020.
- Agrupar estados com comportamento similar para identificar quais estão mais saturados e quais oferecem maiores oportunidades de crescimento.

---

## 🗂️ **Estrutura do Repositório**  

- **01_Base_de_Dados**: Contém os arquivos de dados utilizados para análise.  
- **02_Analise**: Contém o arquivo Jupyter Notebook com a análise e modelagem.  
- **03_Recursos**: Contém recursos visuais utilizados no projeto (imagens e diagramas).  

---

## 💾 **Demonstração e Uso**  

Você pode explorar a análise de duas formas:  

1. **Visualização Direta no GitHub:**  
   - Acesse a pasta **02_Analise** e abra o notebook **real-estate-opportunities-analysis.ipynb** diretamente no GitHub.  
   - [Clique aqui para acessar a análise](https://github.com/tnleite/real-estate-opportunities-analysis/blob/main/02-Analise/real-estate-opportunities-analysis.ipynb).  

2. **Execução Local:**  
   - Clone o repositório e instale as dependências usando o arquivo `requirements.txt`:  
     
   - Abra o notebook no Jupyter ou em uma plataforma de sua preferência e execute as células sequencialmente para explorar as análises.

---

## 🔍 **Estrutura do Projeto**  

### **Parte 1: Coleta e Preparação de Dados**  
- Extração de dados do IBGE e API SIDRA sem bibliotecas externas.  
- Uso de interpolação para ajuste das faixas etárias aos intervalos requeridos.  

### **Parte 2: Análise Exploratória de Dados (EDA)**  
- Visualização da evolução dos consumidores ao longo do tempo por estado.  
- Análise de correlações para identificar fatores relevantes.  

### **Parte 3: Modelagem Preditiva**  
- Aplicação de modelos **XGBoost**, **CatBoost** e **LightGBM** para previsão dos anos de **2021** e **2022**.  
- Avaliação dos modelos com base em métricas de erro, como **RMSE**, **MAE** e **R²**.

### **Parte 4: Clusterização**  
- Uso de K-Means, Agglomerative Clustering e DBSCAN para agrupar estados.  
- Escolha do modelo final com base nas métricas de Silhouette e Davies-Bouldin.  
- Interpretação dos clusters para identificação de estados saturados e com oportunidades.  

---

## 🏗️ **Arquitetura e Fluxo de Análise**  
<img src="03-Recursos/arquitetura_dados.png">

O fluxo segue a estrutura a seguir:  

1. **Coleta de Dados:** Importação e preparação de dados históricos.  
2. **Manipulação e Limpeza:** Tratamento de inconsistências e valores ausentes com **Pandas**.  
3. **Visualização:** Gráficos exploratórios com **Matplotlib** e **Seaborn**.  
4. **EDA:** Entendimento inicial dos padrões regionais e temporais.  
5. **Modelagem Preditiva:** Previsão dos próximos períodos usando séries temporais e regressão.  
6. **Clusterização:** Agrupamento dos estados com perfis semelhantes de evolução no mercado.  
7. **Insights:** Identificação de oportunidades futuras e recomendações estratégicas.  

---

## 📈 **Impacto e Resultados**

- **Identificação de Oportunidades de Mercado:** Descobrimos os estados com maior potencial de crescimento para direcionamento de ações comerciais, campanhas de marketing e investimentos no setor imobiliário.  
- **Clusters Estratégicos:** Agrupamos os estados brasileiros em perfis claros e acionáveis, identificando aqueles com alta demanda emergente, crescimento estável e saturação de mercado.  
- **Projeções de Crescimento Consistentes:** Por meio da modelagem preditiva, fornecemos estimativas confiáveis de crescimento de consumidores para os anos de 2021 e 2022, permitindo planejamento de longo prazo.  
- **Decisões Baseadas em Dados:**  
  - **Estados Emergentes:** Prioridade para campanhas de marketing e desenvolvimento de novos projetos.  
  - **Estados em Crescimento Estável:** Monitoramento contínuo e investimentos moderados.  
  - **Estados Saturados:** Ajuste de estratégias para evitar superoferta e otimização de portfólio de imóveis.  

Este projeto oferece uma base analítica para apoiar o setor imobiliário em suas decisões estratégicas, minimizando riscos e maximizando retornos em regiões de alto potencial.

---

## 🛠️ **Tecnologias Utilizadas**  

- [Python](https://www.python.org/)  
- [Jupyter Notebook](https://jupyter.org/)  
- [Pandas](https://pandas.pydata.org/)  
- [NumPy](https://numpy.org/)  
- [Matplotlib](https://matplotlib.org/)  
- [Seaborn](https://seaborn.pydata.org/)  
- [Scikit-Learn](https://scikit-learn.org/)  
- [LightGBM](https://lightgbm.readthedocs.io/)  
- [CatBoost](https://catboost.ai/)  

---

## 🖼️ **Screenshots**  

Aqui estão algumas capturas de tela das análises:  

<p align="center">
<img src="03-Recursos/img_analise_01.png" alt="Análise 1">
</p>  
<p align="center">
<img src="03-Recursos/img_analise_02.png" alt="Análise 2">
</p>  
<p align="center">
<img src="03-Recursos/img_analise_03.png" alt="Análise 3">
</p>  

---

## 📞 **Contato**  

- 📫 [thiago.leit@hotmail.com](mailto:thiago.leit@hotmail.com)  
- 💼 [LinkedIn](https://www.linkedin.com/in/tnleite/)  
- ✍🏻 [Medium](https://medium.com/@thiago.leit)  
- 🌐 [Portfólio](https://thiagoleitedata.com.br)  

<p align="left">
<a href="mailto:thiago.leit@hotmail.com"><img src="https://img.shields.io/badge/Email-DF0000?style=for-the-badge&labelColor=212121&logo=maildotru&logoColor=DF0000" target="_blank"></a>
<a href="https://www.linkedin.com/in/tnleite/"><img src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&labelColor=212121&logo=linkedin&logoColor=0A66C2" target="_blank"></a>
<a href="https://wa.me/+5521964105121"><img src="https://img.shields.io/badge/WHATSAPP-25D366?style=for-the-badge&labelColor=212121&logo=whatsapp&logoColor=25D366" target="_blank"></a>
<a href="https://medium.com/@thiago.leit"><img src="https://img.shields.io/badge/MEDIUM-000000?style=for-the-badge&labelColor=FFFFFF&logo=medium&logoColor=000000" target="_blank"></a>
</p>