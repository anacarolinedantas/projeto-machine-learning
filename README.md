# Um estudo sobre a satisfação de passageiros de companhias aéreas
Projeto desenvolvido durante a disciplina de Aprendizado de Máquina do curso de Bacharel em Tecnologia da Informação (UFRN). O principal objetivo do projeto foi analisar como os métodos e técnicas supervisionados vistos durante as aulas se comportam em comitês de classificadores, em uma aplicação prática.

## Base de Dados
Os dados foram obtidos pela plataforma Kaggle, onde são dados de uma pesquisa sobre a satisfação de passageiros de companhias aéreas. Essa base de dados contém 129.880 observações e 24 variáveis, incluindo ID do passageiro, serviço de bordo, limpeza, atraso de partida e chegada etc. Em que os passageiros atribuíram notas numa escala de 0 a 5. Sendo a variável de interesse o Nível de satisfação da companhia aérea (satisfeito e neutro ou insatisfeito).

## Pré-processamento
### Limpeza de Dados
* Removidos 393 dados faltosos
* O banco de dados não possui outliers

### Transformação de dados
* Transformação de atributos nominais para numéricos

### Redução de Dados
* Redução de instâncias
  - Dados faltantes: 129.880 para  129.487 instâncias;
  - Método da amostragem: 129.880 para 14.752 instâncias.
* Seleção de Atributos
  - Correlação de Pearson;
  - Redução de 24 para 6 atributos.
* Extração de Atributos
  - Método PCA;
  - Redução de 24 para 4 atributos.

## Modelos utilizados
Foram realizadas análises utilizando os seguintes métodos e técnicas de aprendizado:
* Aprendizado Supervisionado
  - K-NN
  - Árvore de decisão
  - Naive Bayes
  - Redes Neurais
 
* Aprendizado Não-Supervisionado
  - K-Means
  - Hierárquico Aglomerativo
  - Expectation Maximization (EM)
