# Análise de Estoque de Supermercado com Streamlit
Este projeto demonstra como analisar dados de estoque de supermercado usando Python com as bibliotecas Pandas, Matplotlib, Seaborn e Streamlit. O objetivo principal é visualizar a quantidade de produtos em estoque por categoria, com foco no aprendizado da biblioteca Streamlit para criação de aplicativos web interativos.

# Funcionalidades
* Carregamento de Dados: Carrega dados de produtos de um arquivo CSV (estoque.csv).
* Análise Exploratória: Exibe informações básicas sobre os dados, como número de produtos, categorias únicas e estatísticas    descritivas (através da tabela interativa).
* Visualização de Dados:
  * Gráfico de barras interativo mostrando a quantidade de produtos por categoria.
  * Tabela de dados interativa com opção de filtro por categoria e seleção da quantidade de linhas a serem exibidas.
* Interface Interativa com Streamlit:
  * Permite selecionar categorias para filtrar os dados na tabela e no gráfico.
  * Permite ajustar a quantidade de linhas exibidas na tabela.
  * Exibe os gráficos de forma interativa em um aplicativo web.

# Bibliotecas Utilizadas
* Pandas: Para manipulação e análise de dados tabulares.
* Matplotlib e Seaborn: Para criação de gráficos e visualizações.
* Streamlit: Para criação da interface web interativa.

# Como Executar
1. Instale as dependências:

```
pip install pandas matplotlib seaborn streamlit
```

2. Prepare seus dados:
* Certifique-se de ter um arquivo CSV chamado estoque.csv com os dados dos produtos.
* O arquivo deve conter colunas como "Categoria", "Produto" e "Quantidade".

3. Execute o aplicativo Streamlit:

```
streamlit run seu_script.py
```

* Substitua seu_script.py pelo nome do seu arquivo Python.

4. Acesse o aplicativo:
O Streamlit irá abrir um navegador web com o aplicativo em execução.

# Estrutura do Projeto
* seu_script.py: O arquivo principal do aplicativo Streamlit.
* estoque.csv: O arquivo com os dados dos produtos.
  
# Funcionalidades do Código
* mostra_qntd_linhas(dataframe):
  * Permite ao usuário selecionar a quantidade de linhas a serem exibidas na tabela através de um slider na barra lateral.
  * Exibe o DataFrame com a quantidade de linhas selecionada, formatando a coluna "Valor" para exibir duas casas decimais.
* plot_estoque(dataframe, categoria):
  * Cria um gráfico de barras mostrando a quantidade de produtos em estoque para uma determinada categoria.
  * Utiliza Seaborn para criar o gráfico com um layout visualmente agradável.
  * Rotaciona o nome dos produtos no eixo x para melhor visualização.
* Interface Streamlit:
  * Título e descrição do projeto.
  * Barra lateral com filtros para tabela e gráfico:
    * Checkbox para mostrar/ocultar a tabela.
    * Selectbox para selecionar a categoria a ser exibida na tabela.
    * Slider para selecionar a quantidade de linhas da tabela.
    * Selectbox para selecionar a categoria a ser exibida no gráfico.
  * Exibe a tabela filtrada e o gráfico interativo.

# Observações
* Este é um projeto básico para fins de aprendizado.
* Os dados utilizados são fictícios e servem apenas como exemplo.
* A interface do Streamlit pode ser personalizada para melhorar a experiência do usuário.
