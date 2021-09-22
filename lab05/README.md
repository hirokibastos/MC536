# MC536-lab05
Laboratório 05, MC536 - Bancos de Dados Teoria e Prática, UNICAMP, 2S2021
## Aluno
* 176573: Renan Hiroki Bastos

## Tarefa de Cypher sobre Marcadores e Taxonomia

## Tarefa 1

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, sem considerar as categorias subordinadas.

### Resolução
~~~cypher
MATCH (c:Categoria {id:"Serviços"})<-[:Pertence]-(m:Marcador)
RETURN m
~~~

## Tarefa 2

Escreva em Cypher uma consulta que retorne os marcadores da categoria `Serviços`, considerando as categorias subordinadas.

### Resolução
~~~cypher
MATCH (c:Categoria {id:"Serviços"})

MATCH (c1:Categoria)-[:Superior]->(c)

MATCH (c2:Categoria)-[:Superior]->(c)
MATCH (c3:Categoria)-[:Superior]->(c2)
	
MATCH (m:Marcador)-[:Pertence]->(c)
MATCH (m1:Marcador)-[:Pertence]->(c1)
MATCH (m3:Marcador)-[:Pertence]->(c3)

RETURN m, m1, m3
~~~