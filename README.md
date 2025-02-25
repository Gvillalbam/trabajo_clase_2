1) Qué es, que aplicaciones tiene y como implemento en postgres Bases de Datos Vectoriales?
PostgreSQL
PostgreSQL, comúnmente pronunciado "Post-GRES", es una base de datos de código abierto que tiene una sólida reputación por su fiabilidad, flexibilidad y soporte de estándares técnicos abiertos. A diferencia de otros RDMBS (sistemas de gestión de bases de datos relacionales), PostgreSQL soporta tipos de datos relacionales y no relacionales. Esto la convierte en una de las bases de datos relacionales más compatibles, estables y maduras disponibles actualmente.
Desarrollada originalmente en 1986 como continuación de INGRES (un proyecto de base de datos relacional SQL de código abierto que comenzó a principios de la década de 1970), POSTGRES, ahora conocida como PostgreSQL, fue una creación de Michael Stonebraker, profesor de informática en Berkeley. En 1994, el proyecto agregó soporte para SQL y, poco después, surgió PostgreSQL.
Hoy, PostgreSQL continúa evolucionando, mantenido por un equipo internacional apasionado por mejorar con regularidad este proyecto de base de datos de código abierto y gratuito.

¿Por qué usar PostgreSQL?
Mantener sistemas de bases de datos dinámicos es fundamental en el panorama digital actual, especialmente considerando la velocidad a la que surgen nuevas tecnologías. PostgreSQL es expandible y versátil, por lo que puede soportar rápidamente una variedad de casos de uso especializados con un poderoso ecosistema de extensión, que abarca desde tipos de datos de series de tiempo hasta análisis geoespaciales.
Su diseño versátil y accesible convierte a PostgreSQL en una solución de "talla única" para muchas empresas que buscan formas rentables y eficientes de mejorar sus sistemas de gestión de bases de datos. Creada como una solución de base de datos de código abierto , PostgreSQL está completamente libre de restricciones de licencia, potencial de bloqueo de proveedores o riesgo de implementación excesiva. Los desarrolladores expertos y las empresas comerciales que son conscientes de las limitaciones de los sistemas de bases de datos tradicionales apoyan firmemente PostgreSQL. Trabajan diligentemente para proporcionar el mejor sistema en su clase de gestión de bases de datos relacionales probado sobre el terreno.

Ventajas
Después de más de dos décadas, PostgreSQL sigue siendo una de las bases de datos relacionales disponibles más conocidas y con más soporte. Como tal, PostgreSQL ofrece una serie de beneficios a los desarrolladores que buscan crear entornos de computación altamente escalables en sus infraestructuras locales y basadas en Cloud.
1.	Rendimiento y escalabilidad
 
En sistemas de bases de datos más grandes donde la autenticación de datos y las velocidades de lectura/escritura son esenciales, PostgreSQL es difícil de superar. PostgreSQL soporta diferentes optimizaciones de rendimiento que normalmente solo se encuentran en la tecnología de base de datos patentada, como el soporte geoespacial y la concurrencia sin restricciones. Esto hace que PostgreSQL sea extremadamente eficiente cuando se ejecuta un análisis de datos extenso y profundo en múltiples tipos de datos.
2.	Soporte de concurrencia
 
Cuando varios usuarios acceden a los datos al mismo tiempo, los sistemas de bases de datos tradicionales normalmente bloquean el acceso a los registros para evitar conflictos de lectura/escritura. PostgreSQL gestiona la concurrencia de manera eficiente mediante el uso de MVCC (Control de concurrencia de múltiples variantes). En la práctica, esto significa que las lecturas no bloquean las escrituras y las escrituras no bloquean las lecturas.
3.	Soporte de lenguaje profundo
 
PostgreSQL es una de las bases de datos más flexibles para desarrolladores debido a su compatibilidad y soporte de múltiples lenguajes de programación. Los lenguajes de codificación populares como Python, JavaScript, C/C ++, Ruby y otros ofrecen un soporte maduro para PostgreSQL, lo que permite a los desarrolladores realizar tareas de bases de datos en el lenguaje que dominan sin generar conflictos en el sistema.
4.	Continuidad del negocio
 
Las empresas deben mantener operaciones continuas en caso de desastres. Requieren una solución sostenible para garantizar que las bases de datos de producción permanezcan disponibles tanto para los clientes como para los desarrolladores en todo momento. PostgreSQL se puede configurar para garantizar una alta disponibilidad de servicios a través de métodos de replicación asíncronos o síncronos en varios servidores.
5.	100 % de código abierto
 
La implementación de tecnología de gestión de bases de datos de código abierto ofrece beneficios únicos a las empresas, incluidos mejores costos, mayor flexibilidad e innovación que no siempre está disponible con las soluciones de bases de datos patentadas. Desarrollado por un grupo diverso de colaboradores, PostgreSQL se basa en una base sólida de conocimiento, experiencia y valores de código abierto, lo que la convierte en la base de datos más avanzada del mundo.
Funciones
Los desarrolladores experimentan una serie de beneficios al usar PostgreSQL en implementaciones de bases de datos empresariales. PostgreSQL viene con una gran cantidad de funciones y extensiones para crear bases de datos altamente escalables y fáciles de administrar, al tiempo que proporciona una replicación y concurrencia sin problemas en múltiples entornos de cómputo.

6.	Recuperación en un punto temporal determinado
 PostgreSQL permite a los desarrolladores usar PITR (Point-In-Time Recovery) para restaurar bases de datos a un momento específico en el tiempo cuando se realizan acciones de recuperación de datos. Debido a que PostgreSQL mantiene un registro de escritura anticipada (WAL) en todo momento, registra cada cambio en la base de datos. Esto facilita la restauración de los sistemas de archivos a un punto de partida estable.
Herramientas de terceros como pgBackRest (enlace externo a ibm.com) hace que esto sea más fácil de realizar y más fiable; la mayoría de los servicios PostgreSQL gestionados en Cloud se encargarán de esto automáticamente.
7.	Procedimientos almacenados
 PostgreSQL presenta soporte integrado para múltiples lenguajes de procedimiento, lo que ofrece a los desarrolladores la capacidad de crear subrutinas personalizadas llamadas procedimientos almacenados. Estos procedimientos se pueden crear e invocar en una base de datos determinada. Con el uso de extensiones, los lenguajes de procedimiento también se pueden utilizar para el desarrollo en muchos otros lenguajes de programación, incluidos Perl, Python, JavaScript y Ruby.

Aplicaciones de PostgreSQL 
1.	Aplicaciones de Servidor PostgreSQL 
A continuación, se tiene una lista de aplicaciones de servidor PostgreSQL y utilidades de soporte. Estos comandos sólo se pueden ejecutar de manera útil en el host donde reside el servidor de la base de datos.

initdb — create a new PostgreSQL database cluster
pg_archivecleanup — clean up PostgreSQL WAL archive files
pg_checksums — enable, disable or check data checksums in a PostgreSQL database cluster
pg_controldata — display control information of a PostgreSQL database cluster
pg_createsubscriber — convert a physical replica into a new logical replica
pg_ctl — initialize, start, stop, or control a PostgreSQL server
pg_resetwal — reset the write-ahead log and other control information of a PostgreSQL database cluster
pg_rewind — synchronize a PostgreSQL data directory with another data directory that was forked from it
pg_test_fsync — determine fastest wal_sync_method for PostgreSQL
pg_test_timing — measure timing overhead
pg_upgrade — upgrade a PostgreSQL server instance
pg_waldump — display a human-readable rendering of the write-ahead log of a PostgreSQL database cluster
pg_walsummary — print contents of WAL summary files
postgres — PostgreSQL database server

2.	Aplicaciones de Client PostgreSQL 
A continuación, se tiene una lista aplicaciones y utilidades cliente de PostgreSQL. No todos estos comandos son de utilidad general; algunos pueden requerir privilegios especiales. La característica común de estas aplicaciones es que pueden ejecutarse en cualquier host, independientemente de dónde resida el servidor de la base de datos.

Cuando se especifican en la línea de comando, los nombres de usuario y de base de datos conservan sus mayúsculas y minúsculas; la presencia de espacios o caracteres especiales puede requerir comillas. Los nombres de tablas y otros identificadores no conservan sus mayúsculas y minúsculas, excepto cuando estén documentados, y es posible que sea necesario citarlos.
clusterdb — cluster a PostgreSQL database
createdb — create a new PostgreSQL database
createuser — define a new PostgreSQL user account
dropdb — remove a PostgreSQL database
dropuser — remove a PostgreSQL user account
ecpg — embedded SQL C preprocessor
pg_amcheck — checks for corruption in one or more PostgreSQL databases
pg_basebackup — take a base backup of a PostgreSQL cluster
pgbench — run a benchmark test on PostgreSQL
pg_combinebackup — reconstruct a full backup from an incremental backup and dependent backups
pg_config — retrieve information about the installed version of PostgreSQL
pg_dump — extract a PostgreSQL database into a script file or other archive file
pg_dumpall — extract a PostgreSQL database cluster into a script file
pg_isready — check the connection status of a PostgreSQL server
pg_receivewal — stream write-ahead logs from a PostgreSQL server
pg_recvlogical — control PostgreSQL logical decoding streams
pg_restore — restore a PostgreSQL database from an archive file created by pg_dump
pg_verifybackup — verify the integrity of a base backup of a PostgreSQL cluster
psql — PostgreSQL interactive terminal
reindexdb — reindex a PostgreSQL database
vacuumdb — garbage-collect and analyze a PostgreSQL database



Implementación en PostgreSQL:
Para implementar bases de datos vectoriales en PostgreSQL, utilizamos extensiones como pgvector. Esta extensión agrega soporte para almacenar y consultar vectores (listas de números) de manera eficiente. Los vectores se utilizan en tareas como búsqueda semántica, sistemas de recomendación y análisis de imágenes, entre otras aplicaciones.
Pasos para implementar pgvector en PostgreSQL:
1. Instalar PostgreSQL y la extensión pgvector
Primero, asegúrate de tener PostgreSQL instalado en tu sistema. Si no lo tienes, puedes instalarlo siguiendo las instrucciones en el sitio oficial de PostgreSQL.
Para instalar la extensión pgvector:
a.Instalar PostgreSQL (si aún no está instalado):
o	En sistemas Ubuntu/Debian:
sudo apt update
sudo apt install postgresql postgresql-contrib

b. Instalar pgvector:
•	Primero, instala las herramientas necesarias para compilar extensiones:
sudo apt install postgresql-server-dev-13
•	Luego, clona el repositorio de pgvector e instala la extensión:
git clone https://github.com/pgvector/pgvector.git
cd pgvector
make && sudo make install
c.Habilitar la extensión pgvector en tu base de datos:
•	Conéctate a tu base de datos PostgreSQL:
bash    
psql -U postgres
•	Crea la base de datos (si aún no la tienes) y habilita la extensión:
CREATE DATABASE vector_db; \c vector_db CREATE EXTENSION pgvector;



2. Crear una tabla con columnas para vectores
Una vez que la extensión está habilitada, puedes crear tablas que incluyan columnas para almacenar vectores. Los vectores se almacenan en tipo de datos vector, y puedes especificar la dimensión del vector.
Ejemplo de creación de una tabla que almacene vectores de dimensión 300:
CREATE TABLE items ( id SERIAL PRIMARY KEY, name TEXT, description TEXT, embedding VECTOR(300) -- Esta columna almacena el vector (por ejemplo, de 300 dimensiones) );

3. Insertar datos (vectores) en la tabla
Los vectores generalmente se generan usando modelos de machine learning (por ejemplo, Word2Vec, BERT, o modelos para imágenes), pero aquí te muestro cómo insertar vectores manualmente. Los valores de los vectores deben representarse como un arreglo de números flotantes.
INSERT INTO items (name, description, embedding) 
VALUES 
  ('Product 1', 'A description of Product 1', '[0.12, 0.34, 0.56, ..., 0.98]'::vector),
  ('Product 2', 'A description of Product 2', '[0.45, 0.67, 0.23, ..., 0.76]'::vector);

4. Crear un índice para optimizar las consultas de similitud
Para realizar búsquedas eficientes de similitudes entre vectores, se recomienda crear un índice sobre la columna que almacena los vectores. Esto ayuda a realizar consultas de k-NN (k-nearest neighbors) de manera más rápida.
CREATE INDEX ON items USING ivfflat (embedding vector_l2_ops) WITH (lists = 100);

El índice ivfflat usa una estructura basada en el algoritmo de particionamiento para acelerar las búsquedas de similitud.
5. Realizar consultas de similitud (k-NN)
Ahora puedes hacer consultas de similitud para encontrar los vectores más cercanos a un vector de consulta. Por ejemplo, si tienes un nuevo vector de consulta y deseas encontrar los 5 productos más similares en términos de su vector:
SELECT id, name, embedding <=> '[0.12, 0.34, 0.56, ..., 0.98]'::vector AS distance
FROM items
ORDER BY distance
LIMIT 5;
En esta consulta:
•	<=> es el operador utilizado para calcular la distancia entre el vector de consulta y los vectores almacenados.
•	distance es la distancia calculada entre el vector de consulta y los vectores en la base de datos.
•	LIMIT 5 limita los resultados a los 5 vectores más cercanos.




2) 2) Qué es y que aplicaciones tienen los Datalakes?

Un Data Lake es como un gran almacén donde puedes guardar todo tipo de datos, ya sean estructurados (como bases de datos), semiestructurados (como archivos JSON) o no estructurados (como videos y textos). La magia de los Data Lakes es que no necesitas procesar o estructurar los datos antes de almacenarlos. Puedes guardarlos tal cual y procesarlos cuando los necesites.

Aplicaciones de los Data Lakes
Los Data Lakes tienen muchas aplicaciones interesantes:

Análisis de Big Data: Las empresas pueden almacenar y analizar grandes volúmenes de datos para tomar decisiones más informadas. Por ejemplo, Amazon utiliza Data Lakes para analizar el comportamiento de compra de sus clientes y mejorar sus recomendaciones de productos.

Machine Learning y AI: Los datos en un Data Lake pueden ser utilizados para entrenar modelos de Machine Learning y AI. Por ejemplo, Netflix utiliza Data Lakes para mejorar sus algoritmos de recomendación de contenido.

Integración de Datos: Los Data Lakes permiten integrar datos de diversas fuentes, como sensores IoT, redes sociales y sistemas transaccionales. Un ejemplo es General Electric, que utiliza Data Lakes para monitorear y analizar datos de sus máquinas industriales.

Análisis en Tiempo Real: Los Data Lakes permiten el análisis en tiempo real de los datos, lo que es útil para aplicaciones que requieren respuestas inmediatas, como la detección de fraudes. Por ejemplo, PayPal utiliza Data Lakes para detectar transacciones fraudulentas en tiempo real.

Business Intelligence: Ayudan a las empresas a identificar tendencias y patrones en los datos para mejorar sus estrategias comerciales y operativas. Un ejemplo es , que utiliza Data Lakes para analizar datos de viajes y mejorar sus servicios.


REFERENCIAS
·  PostgreSQL. (n.d.). Documentación oficial de PostgreSQL. Recuperado de https://www.postgresql.org/docs/

·  DigitalOcean. (n.d.). Tutoriales en DigitalOcean. Recuperado de https://www.digitalocean.com/community/tutorials

·  PostgreSQL. (n.d.). PostgreSQL en GitHub. Recuperado de https://github.com/postgres/postgres

•	Google Cloud. (s.f.). ¿Qué es un data lake?. Recuperado de 
cloud.google.com
•	The Data Schools. (s.f.). ¿Qué es un Data Lake? Características principales y sus ventajas. Recuperado de 
thedataschools.com
•	WWWhat's New. (2024, 3 de julio). Qué es un Data Lake y para qué sirve. Recuperado de 
wwwhatsnew.com
* Amazon. (n.d.). What is a Data Lake? Retrieved from AWS.
* Netflix. (2017, February 3). How Netflix built analytics in the cloud with Tableau and AWS. Retrieved from Tableau.
* General Electric. (2014, August 11). GE Announces First Data Lake Approach for Industrial Internet to Better Access, Analyze and Store Industrial-Strength Big Data. Retrieved from GE.
* PayPal. (2023, August 3). The next generation of Data Platforms is the Data Mesh. Retrieved from PayPal Developer.

