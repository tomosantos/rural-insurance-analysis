# Seguro Rural no Paraná: Análise Descritiva (2023)

## Descrição do Projeto
Este projeto realiza uma análise descritiva do mercado de seguro rural no estado do Paraná, utilizando dados de 2023 fornecidos pela base nacional de seguros agrícolas. O objetivo é explorar perfis de apólices, valores de prêmios, subvenções, indenizações e sinistralidade, além de identificar as culturas predominantes e avaliar a sustentabilidade financeira do setor.

## Link para o Artigo Completo
[Análise do Seguro Rural no Paraná em 2023](https://drive.google.com/file/d/11wlnoLtRPPDhPNZ4VW9HNx51vIwt7Hnu/view?usp=sharing)

## Estrutura de Dados
- **Fonte dos Dados**: Planilha Excel `seguro-rural-2023.xlsx` (carregada no notebook `analise_seguro_parana_2023.ipynb`).
- **Variáveis Principais**:
  - `apolice`, `mun`, `nome_mun`, `uf`
  - `seguradora`, `tipo` (custeio, produtividade, florestas, etc.)
  - `cultura`, `tipo_cultura`, `area`, `animal`
  - `prod_est`, `prod_seg`, `nivel_cob`, `total_seg`
  - `premio`, `subvencao`, `taxa`, `indenizacao`
  - `evento`, `sinistro`, `sinistralidade`

## Metodologia
1. Importação e limpeza dos dados com `pandas`.
2. Normalização de categorias de seguro, eventos e culturas.
3. Filtragem para o estado do Paraná (`uf = 'PR'`).
4. Análise estatística descritiva (média, mediana, quartis) das variáveis numéricas.
5. Visualizações com `matplotlib` e `seaborn` (gráficos de barras, pizza, histogramas, boxplots, heatmap e scatter plots).
6. Agrupamentos por cultura para comparação de prêmios, subvenções e indenizações.

## Principais Resultados
- **Distribuição de Prêmios**:
  - Valor mínimo: R$354,26
  - Valor máximo: R$526.126,00
  - Mediana: R$16.810,69
  - Média: R$25.281,86
- **Subvenções**:
  - Mediana: R$4.787,14
  - Média: R$7.587,27
- **Sinistros e Sinistralidade**:
  - 27% das apólices registraram sinistros (média)
  - Sinistralidade média de 24% (razão indenizações/prêmios)
- **Culturas com Mais Apólices**:
  1. Soja (53,1% das apólices)
  2. Milho 2ª safra (28,6%)
  3. Trigo (12,7%)
  - As três principais culturas representam ~95% do total de apólices
- **Sustentabilidade Financeira**:
  - Prêmios totais sempre superiores às indenizações para todas as culturas analisadas, indicando rentabilidade para as seguradoras.

## Visualizações Destacadas
- Gráfico de barras: Top 10 culturas com mais apólices
- Gráfico de pizza: Percentual de apólices por cultura e por tipo de cultura
- Histograma e boxplot: Distribuição dos valores de prêmio
- Heatmap: Matriz de correlação das variáveis numéricas
- Scatter plots: Relações entre pares de variáveis com correlações altas e baixas

## Como Reproduzir
```bash
# Instalar dependências
pip install pandas matplotlib seaborn numpy
# Abrir notebook no Jupyter ou Google Colab
jupyter notebook
```  

Abra o arquivo `analise_seguro_parana_2023.ipynb` para ver o passo a passo completo da análise.
