
# 📊 Clusterização com K-Means

Este projeto demonstra a aplicação do algoritmo **K-Means** para realizar a segmentação de clientes com base em seus hábitos de consumo. Utilizando um conjunto de dados fictício (`Mall_Customers.csv`), o notebook mostra como aplicar o algoritmo, avaliar o número ideal de clusters e visualizar os resultados de forma interativa.

---

## 📁 Dados Utilizados

O conjunto de dados contém informações de clientes, incluindo:

- ID do cliente
- Gênero (removido para simplificação)
- Idade (removida no pré-processamento)
- Renda anual (em milhares de dólares)
- Score de consumo (1-100)

---

## ⚙️ Etapas do Processo

1. **Importação de bibliotecas e leitura do dataset**
2. **Pré-processamento**
   - Remoção de colunas irrelevantes (`Gender`, `CustomerID`, `Age`)
   - Normalização com `StandardScaler` para tratar a diferença de escala entre as variáveis
3. **Clusterização com K-Means**
   - Aplicação do K-Means com 5 clusters
   - Geração dos rótulos (labels) para cada cliente
4. **Visualização dos Resultados**
   - Gráfico de dispersão com Plotly, colorido por cluster
5. **Determinação do número ideal de clusters**
   - Uso do **método do cotovelo** com distorção e inércia para avaliar o melhor valor de K
   - Gráfico do cotovelo para ajudar na escolha

---

## 📈 Visualizações

- Gráfico interativo com Plotly mostrando os clientes agrupados
- Gráfico do método do cotovelo para determinar o número ótimo de clusters

---

## 🛠️ Tecnologias e Bibliotecas

- Python 3
- `pandas`, `numpy` – manipulação de dados
- `scikit-learn` – algoritmo K-Means e pré-processamento
- `matplotlib`, `plotly` – visualização
- `scipy` – cálculo de distâncias para análise da distorção

---

## ✅ Resultados

O algoritmo conseguiu segmentar os clientes com base nos seus perfis de consumo e renda, revelando padrões de comportamento úteis para estratégias de marketing e personalização de ofertas.
