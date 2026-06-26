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

2. **Abra o terminal na pasta do projeto:**
   Navegue até o diretório onde o repositório foi clonado (garantindo que você consegue ver os arquivos `analise_churn.ipynb` e a pasta `data/`).

3. **Instale o Jupyter Notebook (se necessário):**
   Caso utilize uma versão limpa do Miniconda e ainda não possua o ambiente do Jupyter instalado no seu computador, rode o comando abaixo:
   ```bash
   conda install -c conda-forge notebook

4. **Inicie o servidor do Jupyter:**
   No mesmo terminal (garantindo que você está dentro da pasta do projeto), execute o comando abaixo para abrir a interface no seu navegador:
   ```bash
   jupyter notebook

5. **Com a interface do Jupyter aberta:**
   Na interface do Jupyter que se abriu no navegador, clique para abrir o arquivo ECommerceAnalysis.ipynb. Com o notebook aberto, execute as células sequencialmente utilizando Shift + Enter. O Passo 0 do próprio notebook     cuidará de instalar as dependências de análise caso alguma esteja faltando no seu computador. Se não abrir a interface diretamente e estiver tudo certo no terminal abra a url abaixo no navegador:
   ```bash
   http://localhost:8888/tree
   
