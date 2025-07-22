# ebac-previsaodoprecodagasolina

# ⛽ Previsão do Preço da Gasolina - Projeto EBAC

Este projeto foi desenvolvido por **Caroline Carrilho** como parte do curso de Análise de Dados da EBAC. O objetivo foi aplicar técnicas de análise exploratória, pré-processamento e aprendizado de máquina para prever o preço da gasolina no Brasil, com base em dados públicos de 2021.

---

## 📥 1. Coleta de Dados

Os dados foram obtidos da **Agência Nacional do Petróleo (ANP)**, disponíveis publicamente. Foram utilizados dois arquivos CSV, representando o **1º** e **2º semestre de 2021**:

- `ca-2021-01.csv`
- `ca-2021-02.csv`

Devido ao tamanho elevado, as tabelas foram unificadas e uma amostra foi gerada para viabilizar o versionamento no GitHub:

🔗 Arquivo usado: [`gasolina_2021_amostra.csv`](./gasolina_2021_amostra.csv)

---

## 🔍 2. Análise e Pré-Processamento

Após a unificação das tabelas, foi feita a:

- Limpeza de colunas irrelevantes (como endereço e CNPJ).
- Tratamento de dados nulos.
- Conversão da coluna de data e extração de **mês** e **ano**.
- Codificação de variáveis categóricas com **One-Hot Encoding**.
- Separação em variáveis preditoras e alvo (`Valor de Venda`).

---

## 🤖 3. Modelagem

Utilizou-se um modelo de **Regressão Linear**, treinado com 80% dos dados e testado com os 20% restantes.

📊 **Métricas de avaliação:**

- **RMSE**: R$ 0,32  
- **R²**: 0,8810

📌 O modelo mostrou excelente desempenho preditivo no conjunto de teste, explicando cerca de 88% da variação dos preços.

---

## 📊 4. Visualização dos Resultados

Foram feitas visualizações para:

- **Ranking de preços por estado e por município**.
- **Comparação de preço médio por bandeira**.
- **Gráfico de dispersão entre valores previstos e reais**.

Essas visualizações ajudaram a entender onde a gasolina era mais cara, e quais fatores influenciaram os preços.

---

## 💭 5. Conclusão Crítica

**Professor**, eu, **Caroline Carrilho**, avalio que o modelo teve ótimo desempenho dentro do escopo do projeto.  

Como forma de validação prática, simulei a previsão do preço da gasolina em **julho de 2022** na cidade de São Paulo. O modelo estimou **R$ 4,50**, enquanto o preço real foi **R$ 5,78**. A diferença foi atribuída a fatores externos como:

- Aumento da cotação do **dólar**.
- Impactos da **guerra na Ucrânia**.
- Reajustes tributários e inflação no Brasil pós-pandemia.

Isso reforça o quanto fatores **macroeconômicos** impactam preços, e que modelos baseados apenas em dados históricos precisam ser complementados com outras variáveis para projeções mais robustas.

---

## 🔗 6. Acesse o Notebook no Google Colab

Clique no botão abaixo para abrir e executar o projeto completo:

[![Abrir no Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carrilho91/ebac-previsaodoprecodagasolina/blob/main/gasolina_previsao.ipynb)

---

## 🛠️ 7. Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Google Colab
- Git + GitHub

---

📬 **Dúvidas ou sugestões?**  
Fique à vontade para abrir uma issue ou entrar em contato.  
🚀 Obrigada por acompanhar este projeto!
