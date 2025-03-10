# 🔧 Manutenção Preventiva - Machine Learning

## 📌 Descrição do Projeto
Este projeto tem como objetivo a **predição de falhas em máquinas industriais** utilizando **técnicas de Machine Learning**. A partir de dados operacionais das máquinas, aplicamos análise exploratória, tratamento de dados, balanceamento, normalização e testes com diferentes modelos para encontrar a melhor solução para a detecção de falhas.

## 📂 Estrutura do Projeto

```
/
|-- Manutenção_preventiva.ipynb  # Notebook principal com toda a análise e treinamento
|-- dataset.csv                      # Base de dados utilizada no treinamento
|-- modelo_rf.pkl                    # Modelo treinado salvo para uso futuro
|-- requirements.txt                  # Lista de dependências para reprodução do projeto
|-- README.md                         # Documentação do projeto (este arquivo)
```

## 🛠️ Tecnologias Utilizadas
- **Python**
- **Pandas** (tratamento de dados)
- **Matplotlib / Seaborn** (visualização dos dados)
- **Scikit-learn** (modelos de Machine Learning)
- **Imbalanced-learn** (balanceamento dos dados com SMOTE)
- **XGBoost e LightGBM** (testes de modelos avançados)

## 📊 Etapas do Projeto
1️⃣ **Análise Exploratória** - Histograma, boxplots e verificação de outliers
2️⃣ **Tratamento de Dados** - Normalização com MinMaxScaler e StandardScaler
3️⃣ **Balanceamento** - Uso do SMOTE para aumentar a classe minoritária (falhas)
4️⃣ **Treinamento de Modelos** - Random Forest, Decision Tree, XGBoost, LightGBM
5️⃣ **Avaliação** - Métricas como Accuracy, Recall, Precision, F1-score

## 🚀 Como Executar o Projeto
### 📥 1. Clone o repositório:
```bash
git clone https://github.com/araujojv/manutencao_preventiva.git
cd manutencao_preventiva
```

### 📦 2. Instale as dependências:
```bash
pip install -r requirements.txt
```

### ▶️ 3. Execute o notebook:
Abra o **Jupyter Notebook** e rode o arquivo **Manutenção_preventiva.ipynb**:
```bash
jupyter notebook Manutenção_preventiva.ipynb
```

### 💾 4. Para carregar o modelo treinado:
```python
import joblib
modelo = joblib.load("modelo_rf.pkl")
```

## 📌 Resultados
- O **Random Forest** obteve os melhores resultados, com **alta acurácia e recall aprimorado após o balanceamento**.
- **SMOTE** foi utilizado para lidar com o desbalanceamento de classes.
- A normalização e remoção de outliers ajudaram a melhorar o desempenho do modelo.

## 📌 Próximos Passos
🔹 Testar novos hiperparâmetros com `GridSearchCV` para otimizar os modelos
🔹 Implementar uma API para integrar o modelo a sistemas reais
🔹 Criar um dashboard para monitoramento das previsões

