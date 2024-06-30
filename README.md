# Desafio Cientista de Dados - PProductions

## Introdução

Este projeto foi desenvolvido como parte do desafio de Cientista de Dados da Indicium. O objetivo é realizar uma análise de dados cinematográficos para orientar PProductions sobre o tipo de filme que deve ser desenvolvido a seguir.

## Estrutura do Projeto

- `EDA.pdf/`: Contém o PDF com a análise exploratória de dados (EDA).
- `Modelo_preditivo.ipynb/`: Contém o o Jupyter Notebook com o modelo preditivo e a previsão do imdb do filme 'The Shawshank Redemption'.
- `modelo_preditivo_imdb.pkl/`: Contém o modelo salvo em formato `.pkl`.
- `respostas_as_perguntas.pdf/`: Contém a respostas as perguntas dos passos 2 e 3 do desafio em formato PDF.
- `requirements.txt`: Lista de pacotes Python necessários.
- `README.md`: Instruções sobre como instalar e executar o projeto.

## Instalação

1. **Clone o repositório:**

   ```bash
   git clone https://github.com/seuusuario/desafio-cientista-dados.git
   cd desafio-cientista-dados

2. **Crie um ambiente virtual:**

   ```bash
   python -m venv venv
   source venv/bin/activate  # Para Windows: venv\Scripts\activate

3. **Instale os pacotes necessários:**

   ```bash
   pip install -r requirements.txt

## Execução
- `Análise Exploratória de Dados (EDA):/`: Abra o pdf EDA.pdf para visualizar a análise exploratória dos dados.
- `Modelagem Preditiva:/`: O notebook Modelo_preditivo.ipynb contém a modelagem preditiva, incluindo a previsão da nota do IMDB e as variáveis mais importantes.
- `respostas:/`: As respostas das análises estão disponíveis em respostas_as_perguntas.pdf.
- `Modelo Salvo:/`: O modelo preditivo treinado está salvo em modelo_preditivo_imdb.pkl. Você pode carregá-lo em Python para fazer previsões.
  
  ## Carregando o Modelo

Para carregar o modelo salvo e fazer previsões, utilize o seguinte código em Python:

```python
import pickle

with open('models/imdb_rating_model.pkl', 'rb') as file:
    model = pickle.load(file)
