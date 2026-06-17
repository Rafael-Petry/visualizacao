# Relatório

> [!CAUTION]
>
> - Você <ins>**não pode utilizar ferramentas de IA para escrever este relatório**</ins>.

## Identificação

- **Nome:** Rafael Petry da Silva
- **Cartão UFRGS:** 00581131

## Dados utilizados

> [!IMPORTANT]
>
> - Os dados utilizados devem ser informados como **links** para as fontes originais.
> - Se houver mais de um conjunto de dados, liste todos separadamente.
> - Para cada conjunto de dados, inclua também uma **descrição curta** explicando os dados.

1. **Dataset 1:** [Microdados ENEM 2024 - microdados_enem_2024/DADOS/RESULTADOS_2024.csv](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/enem)
    * **Descrição curta:** Dados de resultados obtidos pelos participantes nas provas do ENEM 2024, havendo informações sobre a UF em que a prova foi feita, notas de cada área, etc.

## Código-fonte da visualização

> [!IMPORTANT]
>
> - Indique abaixo onde está, dentro deste repositório, o código-fonte usado para gerar a visualização.

- **Arquivo principal:** [./enem-plot/enem-plot.ipynb](https://github.com/Rafael-Petry/visualizacao/blob/main/enem-plot/enem-plot.ipynb)
- **OBS:** Esse colab espera que o .zip dos microdados esteja no diretório do ambiente. Se o arquivo não for encontrado, ele será baixado da [fonte original](https://download.inep.gov.br/microdados/microdados_enem_2024.zip) usando `curl` com flag -k (insecure) se o usuário confirmar.


## Imagem da visualização gerada

> [!IMPORTANT]
>
> - Insira aqui uma imagem da visualização criada por você. Troque `imagem-da-visualizacao.png` pelo caminho correto do arquivo no repositório. 
> - Se você criou alguma visualização interativa, então descreva aqui como acessá-la. Por exemplo, se for uma página HTML, coloque o link, ou se for uma visualização 3D, descreva como compilar e executar o código. 

<ins>**OBS:**</ins> Foram geradas duas versões da mesma visualização, uma estática como imagem ([./enem-plot/enem-plot.png](https://github.com/Rafael-Petry/visualizacao/blob/main/enem-plot/enem-plot.png)), e outra que possui interação como html ([./enem-plot/enem-plot.html](https://github.com/Rafael-Petry/visualizacao/blob/main/enem-plot/enem-plot.html)). A versão estática é apresentada abaixo.

<img width="800" height="600" alt="enem-plot" src="https://github.com/user-attachments/assets/9ee589ec-a42c-40db-a916-247d4679df29" />

## Descrição da visualização

### Legenda (*caption*)

> [!IMPORTANT]
>
> - Escreva um texto curto explicando como interpretar a visualização. Descreva os elementos visuais, eixos, cores, símbolos ou interações relevantes.
> - Este texto seria a legenda (*caption*) que acompanharia a figura em uma publicação, por exemplo.

Mapa coroplético com bolhas para representar a média simples das notas nas áreas de conhecimento do ENEM (incluindo a redação) de todos participantes qualificados por UF, além da quantidade destes participantes nos Estados. Considera-se como "participante qualificado" qualquer participante que tenha obtido notas em todas áreas e redação maior que 0. Cores mais azuladas na UF representam médias mais acima da média nacional e cores mais avermelhadas são notas mais abaixo. As bolhas possuem volume proporcional à quantidade de participantes qualificados nos Estados. Na versão interativa, passar o _mouse_ em cima de alguma UF apresenta, também, o valor exato da média e da quantidade de participantes qualificados para aquele Estado específico.

### Conclusão demonstrada pela visualização

> [!IMPORTANT]
>
> - Escreva uma conclusão curta sobre os dados com base na visualização.
> - Explique qual insight, padrão ou tendência pode ser observado.

É possível concluir que:

1. Em relação à média nacional, a região que obteve as melhores médias no ENEM de 2024 é a sudeste (seguida da regĩao sul), enquanto que a região com piores médias é a norte (seguida de nordeste).

2. É possível afirmar com maior grau de confiabilidade que os participantes do Estado de São Paulo foram os que obtiveram notas acima da média nacional com maior consistência no ENEM de 2024. Isso pode ser dito porque, apesar de haver outras UFs com médias similares, todos possuem uma amostra (número de participantes) menor do que a de SP, o que reduz a confiabilidade.
