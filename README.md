# Org-o_sofredor 🫀

## Descrição do Projeto

Este projeto realiza uma **análise exploratória de dados (EDA)** sobre doenças cardíacas utilizando o dataset **Heart Disease StatLog**. O objetivo é investigar padrões e correlações entre variáveis clínicas e a presença de doenças cardíacas.

## 📊 Dataset

**Arquivo:** `Heart_disease_statlog.csv`  
**Tamanho:** 270 pacientes × 14 variáveis

### Variáveis do Dataset

| # | Nome | Descrição | Tipo |
|---|------|-----------|------|
| 1 | **age** | Idade do paciente (em anos) | Numérica |
| 2 | **sex** | Gênero (0: Feminino, 1: Masculino) | Nominal |
| 3 | **cp** | Tipo de dor no peito (0-3) | Nominal |
| 4 | **trestbps** | Pressão arterial em repouso (mm/HG) | Numérica |
| 5 | **chol** | Colesterol sérico (mg/dl) | Numérica |
| 6 | **fbs** | Açúcar no sangue em jejum > 120 mg/dl (0/1) | Nominal |
| 7 | **restecg** | Resultado do eletrocardiograma em repouso (0-2) | Nominal |
| 8 | **thalach** | Frequência cardíaca máxima alcançada | Numérica |
| 9 | **exang** | Angina induzida por exercício (0/1) | Nominal |
| 10 | **oldpeak** | Depressão ST induzida por exercício | Numérica |
| 11 | **slope** | Inclinação do segmento ST (0-2) | Nominal |
| 12 | **ca** | Número de vasos principais (0-3) | Nominal |
| 13 | **thal** | Talassemia (0-3) | Nominal |
| 14 | **target** | Presença de doença cardíaca (0: Não, 1: Sim) | Nominal |

## 📈 Análises Realizadas

### 1. **Distribuição de Idades**
- Histograma e Boxplot da idade dos pacientes
- Visualização da dispersão etária na amostra

### 2. **Distribuição por Sexo**
- Contagem e proporção de pacientes por gênero
- Gráfico de pizza mostrando:
  - **67.8%** Masculino (183 pacientes)
  - **32.2%** Feminino (87 pacientes)

### 3. **Tipos de Dor no Peito (cp)**
- Categorização dos tipos de dor:
  - Angina típica
  - Angina atípica
  - Dor não cardíaca
  - Assintomático
- Análise da relação entre tipo de dor e presença de doença cardíaca

### 4. **Pressão Arterial em Repouso (trestbps)**
- Estatísticas descritivas:
  - **Média:** 131.34 mm/HG
  - **Mediana:** 130 mm/HG
  - **Intervalo:** 94 - 200 mm/HG
- Detecção e remoção de outliers usando o método IQR
- Histogramas e boxplots para visualização

### 5. **Colesterol (chol)**
- Distribuição de níveis de colesterol sérico
- Análise de outliers
- Visualização comparativa antes e depois da limpeza dos dados

### 6. **Correlação: Frequência Cardíaca Máxima vs. Idade**
- Scatter plot mostrando a relação entre:
  - **Idade:** 29 - 77 anos
  - **Frequência cardíaca máxima**
- Linha de tendência para visualizar correlação
- Diferenciação por presença/ausência de doença cardíaca

### 7. **Distribuição da Variável Alvo (target)**
- Proporção de pacientes com e sem doença cardíaca
- Base para problemas de classificação

## 🛠️ Tecnologias Utilizadas

```python
- pandas: Manipulação e análise de dados
- numpy: Operações numéricas
- matplotlib: Visualização de gráficos
- seaborn: Visualizações estatísticas avançadas
```

## 📁 Estrutura do Repositório

```
Org-o_sofredor/
├── README.md                              # Este arquivo
├── Bateforteotambor.ipynb                 # Notebook com análise completa
├── Heart_disease_statlog.csv              # Dataset
└── Doenca_Cardiaca_Apresentacao.pptx      # Apresentação dos resultados
```

## 🚀 Como Usar

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/Arzenha/Org-o_sofredor.git
   cd Org-o_sofredor
   ```

2. **Instale as dependências:**
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. **Abra o Jupyter Notebook:**
   ```bash
   jupyter notebook Bateforteotambor.ipynb
   ```

4. **Execute as células** para reproduzir as análises

## 📊 Principais Descobertas

- Forte desbalanceamento entre gêneros na amostra (2.1:1 masculino/feminino)
- Pressão arterial média dentro de faixa de hipertensão (131 mm/HG)
- Correlação negativa entre idade e frequência cardíaca máxima
- Presença de outliers em colesterol e pressão arterial
- Diferentes padrões de sintomas entre pacientes com e sem doença cardíaca

## 👨‍💻 Autor

**Arzenha**

## 📝 Licença

Este projeto está disponível no GitHub sob uma licença aberta.

---

**Nota:** Este é um projeto educacional focado em análise exploratória de dados (EDA) e visualização. Não deve ser utilizado para diagnóstico médico real sem validação profissional adequada.
