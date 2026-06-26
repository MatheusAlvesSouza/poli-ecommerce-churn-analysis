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

O código foi desenvolvido de forma modular e **inteligente**, pensado para que qualquer pessoa consiga rodar sem complicações de ambiente. O fluxo está dividido em:

* **Passo 0: Autogestão de Dependências:** Um bloco dinâmico que verifica se as bibliotecas necessárias estão instaladas no ambiente e efetua o download automático das que estiverem faltando.
* **Passo 1: Carregamento de Dados:** Leitura e estruturação automatizada do arquivo `dataset.csv` com Pandas.
* **Passo 2: Relatório Estatístico:** Consolidação de métricas clássicas em uma única tabela descritiva (Média, Mediana, Moda, Percentis 25/50/75, Mínimo, Máximo, Intervalo, Desvio Padrão, Covariância e Correlação com o Churn).
* **Passo 3: Distribuição Visual (Boxplot):** Gráficos que demonstram visualmente a dispersão, comportamento central e identificação de anomalias (*outliers*).
* **Passo 4: Cruzamento com Regras de Negócio:** Análise segmentada dividindo o comportamento de usuários que cancelaram versus usuários ativos.

---

## 🚀 Como Executar o Projeto Localmente

### Pré-requisitos
Certifique-se de ter o **Anaconda** ou **Miniconda** instalado no seu sistema.

### Passo a Passo

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/SEU-USUARIO/ecommerce-churn-analysis.git](https://github.com/SEU-USUARIO/ecommerce-churn-analysis.git)
   cd ecommerce-churn-analysis
