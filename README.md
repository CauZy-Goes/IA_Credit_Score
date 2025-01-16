# IA para Classificação de Score de Crédito

Este projeto envolve o desenvolvimento e treinamento de modelos de machine learning para classificar o score de crédito dos clientes de um banco como **"poor" (ruim), "good" (bom) ou "standard" (padrão)**. O projeto utiliza a biblioteca **scikit-learn** para o treinamento e avaliação dos modelos, e **NumPy** para o tratamento dos dados. O conjunto de dados utilizado contém informações de clientes, com etapas de pré-processamento para manipulação de dados categóricos e divisão em conjuntos de treino e teste.

## Funcionalidades

- **Pré-processamento de Dados**:
  - Tratamento de dados categóricos usando `LabelEncoder` para converter colunas do tipo "object" em valores inteiros.
  - Divisão do conjunto de dados em treino e teste com `test_size=0.3`.
  - Uso do `NumPy` para manipulação eficiente dos dados.

- **Modelos de Machine Learning**:
  - **Random Forest Classifier**:
    - Acurácia alcançada: **0.8222**
  - **K-Nearest Neighbors (KNN)**:
    - Acurácia alcançada: **0.7332**
  - O Random Forest apresentou melhor desempenho em relação ao KNN.

## Instalação

1. Clone o repositório:
   ```bash
   git clone <repository_url>
   cd <repository_folder>
   ```

2. Crie um ambiente virtual (opcional, mas recomendado):
   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows: venv\Scripts\activate
   ```

3. Instale as dependências necessárias:
   ```bash
   pip install -r requirements.txt
   ```

## Como Usar

1. Coloque o conjunto de dados dos clientes (`.csv`) na pasta do projeto.
2. Execute o script de pré-processamento e treinamento dos modelos:
   ```bash
   main.py
   ```
3. O script irá:
   - Preprocessar os dados.
   - Treinar os modelos Random Forest e KNN.
   - Exibir as respectivas acurácias.

## Arquivos do Projeto

- `main.py`: Script principal para pré-processamento, treinamento e avaliação.
- `requirements.txt`: Lista de dependências do projeto.
- `README.md`: Este arquivo, que fornece uma visão geral do projeto.

## Resultados

| Modelo              | Acurácia |
|---------------------|----------|
| Random Forest       | 0.8222   |
| K-Nearest Neighbors | 0.7332   |

O Random Forest Classifier apresentou melhor desempenho em comparação ao KNN, tornando-se o modelo recomendado para esta tarefa.

## Bibliotecas Utilizadas

- **scikit-learn**: Para implementação dos modelos de machine learning.
- **NumPy**: Para manipulação dos dados.

## Melhorias Futuras

- Experimentar ajustes nos hiperparâmetros de ambos os modelos para melhorar a acurácia.
- Testar modelos adicionais, como Regressão Logística ou Support Vector Machines (SVM).
- Melhorar as etapas de pré-processamento para lidar com dados ausentes ou desbalanceados.

## Contribuições

Contribuições são bem-vindas! Abra uma issue ou envie um pull request caso queira melhorar este projeto.

## Autor

**Cauã Farias**

Fique à vontade para se conectar comigo no [LinkedIn](https://www.linkedin.com/in/cau%C3%A3-farias-739013288/) para discutir este projeto ou qualquer outro assunto relacionado a IA e machine learning!
