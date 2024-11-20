# Previsão de Valores de Reembolso para Estações de Carregamento de Veículos Elétricos

Este projeto utiliza **Machine Learning** para prever o valor do reembolso com base em características das estações de carregamento, como custo, localização e marca. Foram testados diferentes modelos de aprendizado para encontrar a melhor abordagem.

https://youtu.be/4JXDqonKUgk

## 🚀 Tecnologias Utilizadas
- Python 3.10+
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- LightGBM
- TensorFlow/Keras
- Matplotlib

## 📁 Estrutura do Projeto
```
├── dataset/
│   └── delaware_ev_charging_rebates.csv  # Dataset utilizado no projeto
├── notebooks/
│   └── model_training.ipynb             # Código para treinar e avaliar os modelos
├── README.md                             # Documentação do projeto
```

## 📊 Modelos Testados
1. **Regressão Linear**:
   - Modelo base para prever o valor de reembolso com base no custo.
2. **Árvore de Decisão**:
   - Captura relações não lineares.
3. **Random Forest**:
   - Combina várias árvores para melhorar a robustez.
4. **XGBoost**:
   - Algoritmo de Gradient Boosting eficiente.
5. **LightGBM**:
   - Variante leve do Gradient Boosting.
6. **Rede Neural**:
   - Modelo com múltiplas camadas para capturar padrões complexos.

## ⚙️ Como Executar

### 1. **Clone este repositório**
```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```

### 2. **Instale as dependências**
Recomenda-se usar um ambiente virtual:
```bash
python -m venv venv
source venv/bin/activate  # Para Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. **Execute o treinamento**
Acesse o arquivo `model_training.ipynb` no Jupyter Notebook ou outro ambiente de sua preferência e execute as células.

### 4. **Resultados**
Os resultados de desempenho dos modelos são exibidos no final do código e podem ser exportados para tabelas e gráficos.

## 🛠️ Pré-processamento
1. **Variáveis Numéricas**:
   - Escaladas usando `StandardScaler`.
2. **Variáveis Categóricas**:
   - Codificadas com `OneHotEncoder` (exceto em XGBoost, que usa suporte nativo a categorias).

## 📈 Avaliação dos Modelos
Os modelos foram avaliados usando as métricas:
- **Erro Médio Quadrático (MSE)**: Penaliza erros grandes.
- **Coeficiente de Determinação (R²)**: Mede a proporção da variância explicada pelo modelo.

### Exemplos de Desempenho:
| Modelo             | MSE    | R²    |
|--------------------|--------|-------|
| Regressão Linear   | 123.45 | 0.89  |
| Árvore de Decisão  | 110.23 | 0.91  |
| Random Forest      | 102.34 | 0.93  |
| XGBoost            | 98.56  | 0.94  |
| LightGBM           | 97.45  | 0.95  |
| Rede Neural        | 100.67 | 0.92  |

## 📂 Dataset
O dataset utilizado contém as seguintes colunas:
- **Cost of Charging Station**: Custo da estação de carregamento.
- **Rebate Amount**: Valor do reembolso.
- **City**: Cidade de instalação.
- **Charging Station Brand**: Marca da estação.
- **County**: Condado de instalação.
- Entre outros.

### Exemplo de Dados:
| Month | Year | City       | Cost of Charging Station | Rebate Amount |
|-------|------|------------|--------------------------|---------------|
| 6     | 2018 | Hockessin  | 500.0                    | 250.0         |
| 6     | 2018 | Wilmington | 649.0                    | 324.5         |

## 📊 Visualizações
Os resultados incluem gráficos como:
- Dispersão: Previsões vs Valores Reais.
- Histogramas: Distribuição dos Resíduos.
- Barras: Comparação de Métricas (MSE, R²) entre os modelos.

## 📜 Licença
Este projeto está sob a licença MIT. Consulte o arquivo `LICENSE` para mais informações.

## ✉️ Contato
Para dúvidas ou sugestões:
- Nome: [Seu Nome]
- Email: [Seu Email]
- LinkedIn: [Seu LinkedIn]

---

### **Como Usar**
1. Substitua os exemplos de resultados e gráficos pelos valores reais do seu projeto.
2. Ajuste as seções de contato e repositório para refletir suas informações.
3. Adicione um arquivo `requirements.txt` com as bibliotecas necessárias:
   ```plaintext
   pandas
   numpy
   scikit-learn
   xgboost
   lightgbm
   tensorflow
   matplotlib
   ```
