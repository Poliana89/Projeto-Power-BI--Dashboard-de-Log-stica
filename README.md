# Projeto Power BI



<h2>Dashboard de Logística</h2>


<h3> Introdução  </h3>
A área de logística de uma empresa automotiva busca otimizar a eficência e melhorar a satisfação dos clientes através de uma gestão mas precisa das suas operações de transporte, com isso necessitam de uma visão mas detalhada das operações, que permitam análise de rotas , desempenho de transporte e otimização de recursos.


<h3> Objetivo </h3>

Criar dashboard onde irá mostrar os KPIs e métricas da área de logística

<h3>Ferramenta Utilizada</h3>

Usaremos a ferramenta Power BI, na versão desktop Versão: 2.132.908.0 64-bit (agosto de 2024).

<h3>Análise.</h3>

    • On Time Delivery (OTD), Medir o percentual de entregas dentro do prazo. 
    • Quantidades de Viagens, Total de viagens por tipo de veiculo.
    • Evolução do frete, Análise temporal do valor do frete
    • Mapa de rotas, visualizar a malha logística para otimizar as rotas.
    • total de viagens, peso e cubagem, avalizar a eficiência do transporte, analisando o total de viagens, peso e cubagem transportada.
    • Desempenho por região: Performance regional com base nas entregas dentro e fora do prazo

  <h3>Transformando e Tratando o Conjunto de Dados da Logística</h3>


 <b> Carregando a fonte de dados no Power BI– </b> A fonte de dados são dados fictícios na extensão  historico transporte.xlsx e valor do frete.txt.



 Ao importar o arquivo foi verificado á necessidade  de tratar os dados, aberto o PowerQuery e foi feita as seguintes tratativas no arquivo historico transporte.xlsx:
 

    • Remoção das duas primeiras linha do arquivo , estava em branco e sem utilidade para análise 
    • Primeira linha como cabeçalho.
    • Foi separado em colunas os dados que estava juntos "cidade-UF", dividido em colunas Destino-cidade e Destino-UF
    • Usado a função subtrair dias, em adicionar coluna , entre as colunas "Data da entrega" e "Data da coleta" , e nomeado a nova coluna como Prazo Realizado,criado também nova coluna condicional "Status Transporte", para identificar se a entrega está em atraso ou não.



<h3>Construção do Dashboard - Relatório Logística </h3>

<li> Utilizado o gráfico  CARTÃO, passando a coluna <b>Valor_Frete</b>, e realizando a soma de todos os frete,  assim temos o <b>CUSTO TOTAL DE TRANSPORTE</B> . </li>

<li>Utilizado o gráfico  CARTÃO, passando a coluna<b> load</b>, realizando a contagem, assim conseguimos extrair o total de viagens.</li>

<li>Utilizado o gráfico  CARTÃO, passando a coluna<b> cubagem </b>, realizando a soma, assim conseguimos extrair a soma total de cubagem.</li>

<li>Utilizado o gráfico  CARTÃO, passando a coluna<b> peso bruto</b>, realizando a soma do peso bruto, conseguimos extrair a soma total do peso bruto</li>

<li> Utilizado o gráfico de barra empilhada , conseguimos mostrar a performance por região, realizando o drill up e drill down em estado e cidade, mostrando a porcentagem de viagens em atraso e dentro do prazo.</li>
<li> Utilizado o gráfico de barra , conseguimos mostrar viagens por tipo de veiculo (truc, vuc, carreta e toco), quantas viagens cada veiculo realizou </li>

<li> Utilizado o gráfico flow map, para visualizarmos os destinos das viagens de cada origem , dessa forma conseguimos análisar a necessidade de implantar uma base de apoio (CD)  no meio dos percursos, visando diminuir o  tempo de viagem e valor de frete </li>

<li> Utilizado o gráfico de linha , para visualizarmos o aumento do frete ao longo de 2022 á 2023 </li>

<li> Utilizado o gráfico velocímetro, para medir o percentual de entregas dentro do prazo, e adicionando uma meta de 80% de entragas dentro do prazo. .</li>

<br></br>
<b>Filtros:</b> O dashboard irá dar ao usuário a possibilidade de filtrar os dados por data de coleta, transportadora, cidade destino, cidade origem(aplicado esse filtro para o mapa) e tipo de transporte.

<h3>Publicação</h3>

Para visualização do relatório <b> Dashboard Logística</b>, basta clicar no link abaixo.

<a> [https://app.powerbi.com/view?r=eyJrIjoiMjkwY2NlNjQtMzZkMi00ZWQ4LWFiODEtNmZjYmIxMmEzMmU1IiwidCI6IjU1Mjc3NjUwLThhODAtNDVlZC04M2I5LTc0MmU0ZGM5MmY4NiJ9](https://app.powerbi.com/view?r=eyJrIjoiYjBiNDQ3MDQtYjQzNy00YjIxLTg0NjMtMDZmOTA1MmJiMDEzIiwidCI6IjU1Mjc3NjUwLThhODAtNDVlZC04M2I5LTc0MmU0ZGM5MmY4NiJ9)
</a>
