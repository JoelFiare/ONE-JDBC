<h1 align="center"> Proyecto Final Java y JDBC<br>con Base de Datos en MySQL<br>Oracle Next Education</h1>

## Autor:
[Joel Benjamín Fiaré](https://github.com/JoelFiare "Joel Benjamín Fiaré")

### Información:
* Proyecto creado con Maven para manejar las dependencias.

* Con JDBC y el driver de MySQL. Aplique buenas prácticas de desarrollo, y utilice algunos patrones de diseño para optimizar la reutilización del código, como por ejemplo el patrón factory que utilice en la connectionFactory para tomar conexiones con la base de datos.

* Utilice el patrón DAO, que centraliza las operaciones de acceso a un recurso específico. En este caso, tenemos el recurso de categoría, las tablas de la base de datos, que son la categoría y el producto. Y las clases DAO hacen justamente todo ese manejo de las conexiones de acceso a las fuentes de datos.

* Utilice el modelo de arquitectura MVC, Model View Controller, que divide las responsabilidades de las aplicaciones en capas específicas para la vista, el modelo y las reglas de negocio.

* Utilice C3P0 para mantener una buena performance y optimización de recursos de la aplicación a través de la configuración de un pool de conexiones, y lo utilice en la connectionFactory para crear un dataSource que tiene un pool de conexiones.

* Utilice el recurso de try with resources, para no preocuparme de los recursos abiertos. El try with resources utiliza recursos que son AutoCloseable y que se cierran solos como lo indica su nombre para no tener que preocuparnos con estar cerrando las conexiones manualmente.

* Protegí la aplicación de posibles ataques de SQL injection utilizando PreparedStatements en vez de Statement.

* Resolvi el problema de queries N+1 utilizando INNER JOIN para no tener que realizar más de una conexión a la base de datos para buscar todos los recursos que tienen relación entre categoría y producto.

 ## Base de Datos:
 [control_de_stock.sql](https://github.com/JoelFiare/ONE-JDBC/blob/main/resources/control_de_stock.sql)

  ## Vista Previa:
![](https://github.com/JoelFiare/ONE-JDBC/blob/main/resources/Interfaz-01.jpg)
![](https://github.com/JoelFiare/ONE-JDBC/blob/main/resources/Interfaz-02.jpg)


