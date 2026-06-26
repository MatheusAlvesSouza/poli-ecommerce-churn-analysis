# Análise de Churn em E-commerce 📊🛒

Este repositório contém o desenvolvimento do projeto prático para a disciplina **ESW-008 (Engenharia da Informação / Ciência dos Dados)** do PECE - Escola Politécnica da USP (POLI-USP). 

O objetivo principal é explorar, caracterizar e analisar dados comportamentais de clientes de uma plataforma de e-commerce para identificar padrões de cancelamento/abandono de serviço (**Churn**).

---

## 👥 Integrantes do Grupo
* **Igor Testa Ramos**
* **Fernanda Azevedo**
* **Matheus Alves de Souza**
* **Pablo Martins da Versa**

---

## 📌 Sobre o Projeto

Empresas de e-commerce e telecomunicações geram volumes massivos de dados diariamente sobre a jornada do cliente (tempo de navegação, dispositivos conectados, volume de compras, etc.). Este projeto foca em aplicar o **Ciclo de Vida dos Dados** para transformar esses registros brutos em insights de negócios capazes de mitigar a perda de clientes.

### Atributos Focados nesta Etapa:
* `HourSpendOnApp`: Quantidade de horas gastas pelo cliente no aplicativo ou website.
* `NumberOfDeviceRegistered`: Quantidade de dispositivos registrados pelo cliente na plataforma.
* `Churn`: Variável alvo binária (0 = Permaneceu, 1 = Cancelou o serviço).

---

## 🛠️ Estrutura do Notebook (`.ipynb`)

O código foi desenvolvido de forma modular e inteligente, integrado com documentação em Markdown para facilitar a interpretação dos resultados. O fluxo de engenharia e análise de dados está dividido em:

* **Passo 0 e 1: Verificação de Ferramentas e Carregamento:** Um bloco dinâmico que valida o ambiente local, instala bibliotecas ausentes automaticamente e realiza a leitura estruturada do arquivo `dataset.csv` com Pandas.
* **Passo 2: Tratamento de Valores Ausentes (Data Cleaning):** Etapa essencial de qualidade de dados que identifica registros nulos (*NaN*) no atributo `HourSpendOnApp` e os preenche utilizando a mediana da coluna, evitando distorções nas análises.
* **Passo 3: Relatório Estatístico Descritivo:** Consolidação das métricas clássicas em uma única tabela analítica (Média, Mediana, Moda, Percentis 25/50/75, Mínimo, Máximo, Intervalo, Desvio Padrão, Covariância e Correlação com a variável alvo).
* **Passo 4: Matriz de Correlação Visual (Heatmap):** Geração de um Mapa de Calor interativo para avaliar de forma rápida a força e a direção da associação linear entre as variáveis comportamentais e o Churn.
* **Passo 5: Distribuição Visual (Boxplot):** Gráficos de caixa para mapear o comportamento central da massa de usuários, limites operacionais e detecção de anomalias (*outliers*).
* **Passo 6: Cruzamento com Regras de Negócio:** Análise segmentada dividindo visualmente os boxplots entre o grupo de clientes ativos versus clientes que cancelaram o serviço (Churn).

---

## 🚀 Como Executar o Projeto Localmente

### Pré-requisitos
Certifique-se de ter o **Anaconda** ou **Miniconda** instalado no seu sistema.

### Passo a Passo

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/SEU-USUARIO/ecommerce-churn-analysis.git](https://github.com/SEU-USUARIO/ecommerce-churn-analysis.git)
   cd ecommerce-churn-analysis
