[![Python Version](https://img.shields.io/badge/python-3.11.6-blue.svg)](https://www.python.org/downloads/)
![GitHub License](https://img.shields.io/github/license/jrodrigotico/python)

## 	:books: MQO - Método dos Mínimos Quadrados
O Método dos Mínimos Quadrados Ordinários (MQO) é uma técnica estatística amplamente empregada para compreender a relação entre uma variável dependente e uma ou mais variáveis independentes. Reconhecido por sua eficácia na modelagem de problemas lineares, o MQO é crucial em muitos domínios de estudo. 

Neste projeto, o MQO é aplicado para investigar a relação entre quatro variáveis dependentes ('rdpc', 'seg_alimentar', 'subjetividade' e 'serv_essencias') e um conjunto de variáveis independentes. Como resultado, o projeto contém quatro seções distintas dedicadas à análise do MQO para cada uma das variáveis dependentes mencionadas.

Por exemplo:
<p align="center">
  <img src="https://github.com/jrodrigotico/MQO-IBGE/blob/imagens/ols_imagem.png" width=60%>
</p> 




## 	:point_down: Download dos dados no site IBGE
```
- Acessar link: https://www.ibge.gov.br/estatisticas/sociais/saude/24786-pesquisa-de-orcamentos-familiares-2.html?=&t=downloads
- Pesquisa_de_Orcamentos_Familiares_2017_2018
- Microdados
- Dados_20230713.zip
- Extraia dados do zip 'Dados_20230713.zip'
- Selecionar cadernos: 'DOMICILIO.txt', 'CONDICOES_VIDA.txt', 'MORADOR_QUALI_VIDA.txt' e 'MORADOR.txt'

OBS: O Github não aceita upload de dados que superem o tamanho de 25 mb !!!
```

## 	:construction_worker: Tratamento e visualização dos dados
Após baixar os cadernos 'DOMICILIO.txt', 'CONDICOES_VIDA.txt', 'MORADOR_QUALI_VIDA.txt' e 'MORADOR.txt', os dados foram combinados usando a função 'pd.merge' para criar o conjunto principal de dados denominado 'base'. Durante esse processo, realizou-se a verificação de valores ausentes ('NA') e a renomeação de algumas colunas, como 'V6199' para 'SEG_ALIMENTAR_V' e 'V6101' para 'RENDIMENTO_TOTAL', entre outras

As novas variáveis que serão utilizadas no decorrer do código foram criadas utilizando a estrutura condicional 'if' com o auxílio dos métodos 'apply' e 'lambda'. 

Para avaliar a distribuição das variáveis dependentes, como 'rdpc', 'seg_alimentar', 'subjetividade' e 'serv_essencias', foram criados gráficos para visualizar a frequência dos valores '0' e '1', bem como gráficos de frequência relativa dessas variáveis. Além disso, foi gerado um gráfico mostrando a renda média por estado.

Os dados tratados foram submetidos a análises estatísticas como o teste V de Cramer e a correlação de Pearson, a fim de explorar as relações entre as variáveis e identificar possíveis padrões ou associações no conjunto de dados.


## 	:desktop_computer: Clone do repositório
Clone do repositório:

```
git clone https://github.com/jrodrigotico/MQO-IBGE.git
```


## 	:eye: Principais pacotes utilizados
- ``Pandas``
- ``Seaborn``
- ``Scipy stats``
- ``Statsmodels``


## 	:email: Contato
Para feedbacks, sugestão de melhorias ou relato de problemas, sinta-se à vontade para entrar em contato comigo através do meu perfil no Linkedin:

[![LinkedIn Badge](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/joão-rodrigo-lemes-5603a6154/)



