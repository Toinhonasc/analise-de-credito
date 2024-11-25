
# **Projeto: Análise de Crédito**

## **Objetivo**
Desenvolver uma solução para verificar as informações de um cliente e determinar se o crédito pode ser liberado, com base em dados históricos de outros clientes. O sistema utiliza técnicas de Machine Learning para fazer previsões e é implementado com Python.

---

## **Fases do Projeto**

### 1. **Definição do Problema**
- Identificação das variáveis que influenciam a aprovação de crédito.
- Análise dos objetivos de negócio e mapeamento dos critérios de aprovação.

---

### 2. **Preparação dos Dados**
- **Tratamento de Missing Values**: Imputação de valores ausentes utilizando métodos estatísticos ou inferências.
- **Seleção de Features**: Identificação das variáveis mais relevantes para o modelo por meio de análises exploratórias e estatísticas.
- **Categorização**: Transformação de variáveis categóricas em valores numéricos (ex.: One-Hot Encoding).

---

### 3. **Criação do Modelo de Machine Learning**
- **Algoritmo Utilizado**: Random Forest, devido à sua robustez e capacidade de interpretar variáveis categóricas e contínuas.
- **Avaliação de Métricas**:
  - Acurácia
  - Precisão
  - Recall
  - F1-Score
  - Matriz de Confusão

---

### 4. **Colocando em Produção**
- **Framework**: Flask.
- Desenvolvimento de uma API para receber os dados do cliente e retornar a decisão de aprovação ou reprovação do crédito.

---

## **Linguagem e Ferramentas**
- **Linguagem**: Python
- **Bibliotecas Principais**:
  - **pandas**: Manipulação de dados.
  - **numpy**: Operações matemáticas e arrays.
  - **scikit-learn**: Treinamento e avaliação do modelo de Machine Learning.
  - **Flask**: Construção da API para produção.
  - **matplotlib/seaborn**: Visualização de dados.

---

## **Como Executar**

### **Requisitos**
- Python 3.7 ou superior
- Bibliotecas necessárias (disponíveis no arquivo `requirements.txt`):

```bash
pip install -r requirements.txt
```

### **Passos**
1. Clone o repositório:
   ```bash
   git clone <URL_DO_REPOSITORIO>
   cd analise_credito
   ```
2. Execute o script de treinamento do modelo:
   ```bash
   python train_model.py
   ```
3. Inicie o servidor Flask:
   ```bash
   python app.py
   ```
4. Acesse o sistema:
   - URL local: `http://127.0.0.1:5000`
   - Envie os dados do cliente via POST para receber a decisão.

---

## **Próximos Passos**
- Adicionar validação adicional nos dados de entrada da API.
- Integrar a aplicação com um banco de dados para armazenar previsões.
- Implementar pipelines de CI/CD para automatizar a implantação.

