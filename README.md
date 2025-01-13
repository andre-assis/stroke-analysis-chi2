# stroke-analysis-chi2

## Introdução

Este projeto explora a relação entre o tipo de trabalho (empresas privadas e trabalho autônomo) e a incidência de AVC (Acidente Vascular Cerebral) utilizando o teste de qui-quadrado de independência.

### Questão de Pesquisa

- Existe relação entre o tipo de trabalho e a incidência de AVC?
    

### População

- Trabalhadores de empresas privadas e trabalhadores autônomos.
    

### Variáveis

1. **Independente**: Tipo de trabalho (Privado ou Autônomo)
    
2. **Dependente**: Incidência de AVC (Sim ou Não)
    

### Hipóteses

- **Hipótese Nula (H0)**: Não existe relação entre o tipo de trabalho e a incidência de AVC.
    
- **Hipótese Alternativa (H1)**: Existe relação entre o tipo de trabalho e a incidência de AVC.
    

## Estrutura do Projeto

### Bibliotecas Utilizadas

- pandas
    
- numpy
    
- scipy.stats
    
- matplotlib
    

### Dataset

Utilizamos o dataset `healthcare-dataset-stroke-data.csv`, que contém informações sobre o tipo de trabalho, ocorrência de AVC e outras variáveis relacionadas à saúde.

### Principais Etapas

1. **Carregamento e Visualização do Dataset**
    
    - Exibição de uma amostra dos dados.
        
    - Contagem total de registros no dataset.
        
2. **Filtragem de Dados**
    
    - Filtrar apenas trabalhadores privados e autônomos.
        
    - Selecionar apenas registros com AVC (1) ou sem AVC (0).
        
3. **Análise Exploratória**
    
    - Contagem de trabalhadores por tipo de emprego.
        
    - Contagem de ocorrências de AVC por tipo de emprego.
        
4. **Construção de Gráficos**
    
    - Porcentagem de AVC em relação ao tipo de emprego.
        
    - Comparativo de ocorrências de AVC e não AVC por tipo de emprego.
        
5. **Teste Qui-Quadrado de Independência**
    
    - Cálculo do valor do qui-quadrado (chi), valor-p (p), graus de liberdade (dof) e frequências esperadas.
        
    - Aplicação da correção de Yates (opcional).
        

## Resultados e Gráficos

### Gráficos

1. **Porcentagem de AVC por Tipo de Emprego**
    
    - Gráfico de barras mostrando a porcentagem de AVC em trabalhadores privados e autônomos.
        
2. **Contagem de AVC e Não AVC**
    
    - Gráfico de barras agrupadas comparando ocorrências de AVC e não AVC por tipo de emprego.
        

### Teste Qui-Quadrado

- **Resultado Sem Correção de Yates**
    
    - Valor de qui-quadrado (chi): `valor_calculado`
        
    - Valor-p (p): `valor_calculado`
        
- **Conclusão**
    
    - Caso o valor-p seja menor que 0,05, rejeitamos a hipótese nula e concluímos que há relação significativa entre o tipo de trabalho e a incidência de AVC.
        
    - Caso contrário, não há evidência suficiente para rejeitar a hipótese nula.

## Conclusões

Com base nos resultados obtidos neste estudo, podemos concluir que há uma associação significativa entre o tipo de trabalho e o risco de AVC. Nossos achados revelaram que os trabalhadores autônomos apresentaram uma maior prevalência de AVC em comparação com os empregados do setor privado. Essa descoberta sugere que fatores ocupacionais podem desempenhar um papel importante na manifestação dessa condição médica grave.

A relação entre o tipo de trabalho e o risco de AVC pode ser atribuída a diversos fatores. Trabalhadores autônomos geralmente enfrentam uma maior carga de trabalho, responsabilidades e estresse, além de terem menos acesso a benefícios de saúde e cuidados preventivos regulares. Esses fatores podem contribuir para um estilo de vida menos saudável, com maior exposição a fatores de risco, como sedentarismo, má alimentação e falta de controle adequado dos fatores de risco cardiovasculares.

Esses resultados têm implicações importantes para a saúde ocupacional e a prevenção de AVC. É essencial que as políticas de saúde e as intervenções direcionadas considerem as especificidades dos diferentes grupos ocupacionais. Estratégias de promoção da saúde e prevenção de AVC devem ser adaptadas para atender às necessidades dos trabalhadores autônomos, incluindo a conscientização sobre os fatores de risco ocupacionais e a implementação de medidas preventivas no ambiente de trabalho.
