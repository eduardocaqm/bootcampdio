# bootcampdio

SQL - trata-se de uma linguagem de consulta a banco de dados relacionais.
Modelagem relacional já que se trata de dados guardados em tabelas. Necessita de uma estrutura muito rígita,
precisa de um script, com usas chaves primárias e segundárias.
O desenvolvimento de um sistema SQL deve ser muito bem estruturado, já que suas motificações não são impossíveis, mas
são trabalhosas. Logo, quanto mais controle você tem do primeiro passo a ser dado, mais tranquilo é o desenvolvimento do mesmo.

 . Transações - Atomicidade: ou uma transação é executada por completo ou existe um row back, nunca pela metade
		Consistencia: quando uam transação for concluida ele estara em conformidade com as questões pre definidas.
		Isolamento: uma transação nunca influenciara em outra.
		Durabilidade: uma vez a transação concluida, nunca mais esses dados seram pedidos.

NoSQL - criado para ter uma performance melhor e uma escalabilidade mais horizontal para suprir necessidades 
onde os bancos relacionais deixam a desejar. O conceito aplicado trás a ideia
de schema: uma chave de valor é utilizada para recuperar valores, conjunto de colunas ou documentos.

 . Transação - priorização de dados com consistencia em momentos indetermindados.

 A escalabilidade é naturalmente horizontal. Seu particionamento mais comum é o sharding. Permitem um maior desempenho
nas aplicações e tem escalabilidade infinita, claro que conforme o ambiente. Um exemplo dado no bootcamp é um app de comida 
que a noite tem uma movimentação maior e você aumenta o numero de nós nesse determinado momento de pico e então
o diminui em horários diferentes.

algo ruim é ter mais de uma linguagem (as vezes) para um mesmo banco de dados nas consultas.

DIFERENÇAS - O SQL tem dificuldade de conciliar escalabilidade. Já o NoSQL devemos apenas
levar em consideração a modelagem do sistema. Sendo assim, no caso de um sistema simples
a utilização de NoSQL perde a performance quando rodas a aplicação.


Ambos exigem planejamento em seu desenvolvimento, porém, vale ressaltar que o SQL se torna um pouco mais 
rigoroso com sua formatação.

Um ponto forte do SQL é a consistencia das informações.

Com relação a segurança: ambos são sucetíveis a ataques. 

 . documento - documenbtos podem ser descritos como dados no formato de chave-valor
como por exemplo o padrão JSON.
 . colunas - armazenados em linhas particulares de tabela no disco, podendo suportar
várias linhas e colunas, além de permitir sub-colunas. Exemplo: Cassandra.
 . grafos - armazenados em formas de verticés e arestas. Exemplo: Neo4j.
 . chave-valor - a noSQL que mais aguenta carga de dados. Já que a ideia
é que um valor tenha uma chave unica para acesso. Exemplo: Riak.

