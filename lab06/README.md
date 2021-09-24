# MC536 - Lab06 - Artigo de Dataset Público

# Aluno
* `176573`: `Renan Hiroki Bastos`

# Análise do Artigo `BDSmells Data Set: A PL/SQL Code Smell Data Set`

| campo | valor |
|------------|----------------------------------------|
| referência | `de Almeida Filho, F. G., Martins, A. D. F., Vinuto, T. d. S., Monteiro, J. M., de Sousa, I. P., de Castro Machado, J., and Rocha, L. S. (2019). Prevalence of bad smells in pl/sql projects. In Proceedings of the 27th International Conference on Program Comprehension, ICPC ’19, pages 116–121, Piscataway, NJ, USA. IEEE Press.
Fowler, M. (2018). Refactoring: improving the design of existing code. Addison-Wesley Professional.
Karwin, B. (2010). SQL Antipatterns: Avoiding the Pitfalls of Database Programming. Pragmatic Bookshelf, 1st edition.
Khumnin, P. and Senivongse, T. (2017). Sql antipatterns detection and database refactoring process. In 2017 18th IEEE/ACIS International Conference on Software Engineering, Artificial Intelligence, Networking and Parallel/Distributed Computing (SNPD), pages 199–205.
Lanza, M. and Marinescu, R. (2007). Object-oriented metrics in practice: using software metrics to characterize, evaluate, and improve the design of object-oriented systems. Springer Science & Business Media.
McKinney, W. (2010). Data structures for statistical computing in python. In van der Walt, S. and Millman, J., editors, Proceedings of the 9th Python in Science Conference, pages 51 – 56.` |
| link       | `https://drive.google.com/file/d/1Kt95VMdqupj5rm0M7IXxOnvhGSx77aCe/view` |
| dataset | `https://bit.ly/2KNPGv5` |
| formato | `csv` |

## Resumo

Novas ferramentas tornaram possível automatizar o processo de identificação de "Bad Smells" em código SQL, e consequentemente a realização de estudos sobre o assunto. Porém não existia um dataset público para esse propósito. Assim o artigo disponibiliza um dataset chamado BDSmells Data Set, contendo informação sobre "Smells" em código PL/SQL extraido de 20 projetos open source.

O dataset é disponibilizado em um arquivo csv no qual as colunas são os nomes dos projetos e as linhas o ID de cada "code smell". Cada linha tem a soma da acorrencia do "code smell" correspondente através de todos os arquivos de cada projeto.

## Perguntas de pesquisa/análises

Em de Almeida Filho et al. [2019], os autores utilizaram o dataset em estudo sobre a prevalencia de "code smells" de PL/SQL em projetos open source, e concluiram que:
* Alguns "code smells" ocorrem mais que outros, e alguns não ocorreram nenhuma vez no dataset.
* Muitos "code smells" estão relacionados fortemente.
* Os autores exploraram o algoritmo Apriori e encontraram regras de associação indicando que "code smells" de PL/SQL ocorrem juntos.
* Os "code smells" no dataset estão organizados em dois clusters.

## Trabalhos relacionados

**Palomba et al. [2015]**: Autores propuseram uma plataforma web para compartilhamento e validação de data sets de "code smells" chamada LANDFILL.

**Yamashita and Moonen [2013]**: Autores apresentaram um estudo desenhado para prover evidencia empírica sobre como desenvolvedores veem "code smells", com o objetivo de identificar os casos considerados mais relevantes.

**Sharma et al. [2017]**: Autores investigaram as características fundamentais dos "code smells", por meio de um estudo empírico realizado sobre um conjunto de "code smells" que, segundo os autores, são os mais frequentes.

**Outros artigos citados**: Singh and Chopra [2013], Khumnin and Senivongse [2017].
