# RETO_20_2_2017_GGA

Esta tarea consiste en preparar un conector de Presto para Presto. Es decir, conectar un cluster de Presto como uno de los catalogos de otro cluster de Presto. Se supone que se podria hacer modificando el conector JDBC basico que se usa en el conector de MySQL y PostgreSQL (ver https://prestodb.io/faq.html "Does Presto connect to MySQL or PostgreSQL?").

Parece que sera necesario agregar un plugin a Presto. Para ello habria que hacer un fork del repositorio de Presto (https://github.com/prestodb/presto).

En este repositorio hay un docker-compose.yml con el que se levantan dos cluster de Presto, uno de ellos conectado a una base de datos MySQL. El objetivo es agregar el plugin correspondiente al codigo de Presto y usar ese Presto modificado para configurar el otro Presto como catalogo, de manera que en ese Presto modificado se veria la base de datos MySQL a traves del primer Presto. La modificacion del codigo de Presto se quedara en el fork correspondiente y la modificacion del docker-compose.yml debe ponerse en un Pull Request a este repositorio.

Esta tarea puede ser muy complicada, a ver que tal.
