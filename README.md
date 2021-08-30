# Esse jupyter vai ser usado pra dar join nas duas planilhas de cadastro geral.
As seguintes etapas são necessárias.

* Formatar a coluna CPF no formato XXX.XXX.XXX-XX - Feito
* Exclusão de coluna Liberado e Nº na planilha Geral não oficial - Feito 
* Consolidar os dados NaN entre as duas planilhas - Feito
* Adicionar a data da CESTA 1 conforme a "data de entrada" / "data da planilha" - Feito
* Concatenar a os dados em uma planilha só - Feito

### Atualização
 Dado o estranhamento de poucos nomes na planilha resultado do Combine, farei uma analise com dicionarios e validar que todos os nomes foram passados corretamente. Além disso, consolidarei as outras 3 planilhas de cadastro geral antigas que tinhamos no sistema.
 
 ### 16/08/2021
  Devido à organização da planilha final por ordem alfabética, a a coluna Nomes foi ordenada mas as outras colunas não. Isso criou desordem na planilha, já que os dados foram embaralhados.
  
 ### Atualização 30/08/2021
  Erro encontrando, quando as duas planilhas foram combinadas por pd.DataFrame.combine() de alguma forma celulas que eram NaN nas duas planilhas receberam valores de outras celulas.
