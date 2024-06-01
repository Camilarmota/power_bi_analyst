# Desafio criando um Dashboard corporativo com integração com MySQL e Azure
Passos: 

1 - Foi criado uma instância na Azure para MySQL baseado no banco de dados disponível no Github com integração do Power BI e Workbench. 

2 - Foi verificado problemas na base antes de realizar a transformação dos dados. Como a Derrubada a constraint fk_employee ALTER TABLE employee DROP CONSTRAINT fk_employee.

3 - Foi modificado os valores monetários para o tipo double preciso.

4 - Valores sem dados foram preenchidos. 

5 - Foi verificado o número de horas dos projetos: 
  SELECT Pno, SUM(Hours) AS TotalHoras FROM works_on GROUP BY Pno;

Respondendo o porque os dados foram mesclados e não atribuidos, pois o objeivo era tornar o dado único auxiliando na criação do modelo estrela em um módulo futuro.

A mesclagem de dados em vez de atribuir valores diretamente a uma tabela é preferível em muitos casos devido à sua eficiência e flexibilidade. Aqui estão algumas razões pelas quais a mesclagem é uma prática recomendada:
  #### Integridade dos Dados:
  
  A mesclagem de dados permite combinar informações de várias fontes sem comprometer a integridade dos dados existentes na tabela.
  
  #### Atualização de Registros:
  
  Ao mesclar dados, é possível atualizar registros existentes com novas informações, mantendo a consistência dos dados.
  
  #### Evitar Duplicação:
  
  A mesclagem ajuda a evitar a duplicação de dados, garantindo que apenas informações relevantes sejam adicionadas ou atualizadas na tabela.
  
  #### Flexibilidade:
  
  Mesclar dados oferece flexibilidade para combinar informações de diferentes fontes e formatos, adaptando-se a diferentes necessidades de integração de dados.
  
  #### Eficiência:
  
  Em muitos casos, mesclar dados é mais eficiente do que atribuir valores diretamente, especialmente ao lidar com grandes volumes de dados ou operações complexas.
  Portanto, mesclar dados em vez de atribuir valores diretamente a uma tabela é uma prática recomendada para manter a integridade dos dados, evitar duplicações e garantir           eficiência e flexibilidade no processo de integração de dados.


