# Desafio de Projeto  - Modelando um Dashboard de E-commerce com PowerBI Utilizando  Fórmulas DAX

Entrega do Desafio de Projeto, como parte do curso de Análise de Dados  - Klabin - Excel e Power BI Dashboards

# Passo a Passo da Construção do Projeto 

1) Importação do Arquivo em Excel para o PowerBI (ETL);
2) Remoção de todas as relações identificadas pelo PowerBI automaticamente;
3) Transformação dos dados a partir das orientações
* Criação da Tabela Fato, com índice, coluna personalizada ID_Produto, remoção de colunas que constam nas tabelas dimensão;
* Criação das tabelas dimensão, utilizando o processo de criação da coluna personalizada ID_Produto, remoção das colunas que não tinham relações com o objetivo de cada tabela;
* Criação da tabela Calendário no menu de exibição do modelo, através de Fórmulas DAX;
4) Códigos Utilizados
* D_Calendario = CALENDARAUTO(12)
* Ano = (YEAR('D_Calendario'[Date]))
* Número_Mês = (MONTH('D_Calendario'[Date]))
* Número Semana = WEEKNUM('D_Calendario'[Date])
* Dia_da_Semana = WEEKDAY('D_Calendario'[Date])
* Nome_dia_da_semana = FORMAT('D_Calendario'[Date], "DDDD")


