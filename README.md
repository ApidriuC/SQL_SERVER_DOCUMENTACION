<h1 align="center">DOCUMENTACIÓN SQL SERVER</h1>

<p align="justify">Documentación realizada con el objetivo de recordar algunas funcionalidades que nos permite realizar el lenguaje de dominio específico SQL en Microsoft SQL Server Management Studio. A continuación se mostrarán los comandos básicos de CRUD (Create, Read, Update, Delete) y algunas funciones primitivas de SQL Server. Este repositiorio es de proposito educativo.</p>

<p align="justify">

### Usar una base de datos específica	
	
```md
USE *DB*
```

<hr>

### Crear Base de Datos
```md
CREATE DATA BASE *Nombre*
```

<hr>

### Crear una nueva tabla

```md
CREATE TABLE *DATABASE NAME* (
	PK_1 DATA TYPE PRIMARY KEY IDENTITY NOT NULL,
	COLUMN_1 DATA TYPE NOT NULL,
	FK_1 DATA TYPE INT NOT NULL,
	FOREIGN KEY (*FK_1*) REFERENCES *TABLE* (*PK TABLE*) 
)
```

<hr>	

### Seleccionar elementos

```md
SELECT *
FROM *TABLE*
WHERE *CONDITION* 
```

<hr>

### Insertar elementos

```md
INSERT INTO *TABLE*(*COLUMNS*) VALUES (*VALUES*)
```

<hr>

### Actualizar elementos

```md
UPDATE *TABLE* SET *COLUMN* = *VALUE* WHERE *CONDITION* 
```

<hr>

### Borrar elementos de una fila

```md
DELETE FROM *TABLE* WHERE *CONDITION*
```

<hr>

### Borrar columnas de una tabla

```md
ALTER TABLE *TABLE* DROP COLUMN *COLUMN*;
```

<hr>

### Modificar columnas de una tabla

```md
ALTER TABLE *TABLE* ALTER COLUMN *COLUMN* *TIPO DATO*
```

<hr>

### Reiniciar conteo de columnas autoincrementales

```md
DBCC CHECKIDENT (*TABLE*, RESEED, *APARTIR DE (NÚMERO)*)
```

<hr>

### Otorgar Permisos a un Usuario en un Procedimiento Almacenado

```md
GRANT execute on *PROCEDIMIENTO* to *USER*;
```

<hr>

### Reiniciar Columna Identity

```md
DBCC CHECKIDENT (*TABLE*, RESEED, 0)
```

<hr>

### Joins entre tablas

Los "Joins" es el proceso de obtener datos de varias tablas y ponerlos en una vista general. Por lo tanto, la declaración "SQL JOIN" en el comando Select une columnas entre una o más tablas en una base de datos relacional y devuelve un conjunto de datos. Existen varios tipos de "Joins" que veremos a continuación. Cabe resaltar que por defecto el comando "Join" toma la sentencia "Inner".

- Implementación

```md
SELECT *
FROM *TABLE*
*TYPE JOIN* JOIN *TABLE* AS *PSUDONAME* ON *CONDITION JOIN*
WHERE *CONDITION SELECT*
```

- Inner Join:

Toma solo los elementos en común entre la condición establecida

<p align="center">
	<img  alt="" src="https://github.com/ApidriuC/SQL_SERVER_DOCUMENTACION/blob/main/InnerJoin.PNG"></img>	
</p>

<hr>

- Left Join:

Este tipo de unión significa que solo retornan todos los datos de la tabla de la mano izquierda, solo si los datos coinciden con la tabla de la mano derecha

<p align="center">
	<img  alt="" src="https://github.com/ApidriuC/SQL_SERVER_DOCUMENTACION/blob/main/LeftJoin.PNG"></img>	
</p>

<hr>

- Right Join:

Este tipo de unión es el caso opuesto al anterior. Implica que solo retornaran los datos de la tabla de la mano derecha, solo si los datos coinciden con la tabla de la mano izquierda

<p align="center">
	<img  alt="" src="https://github.com/ApidriuC/SQL_SERVER_DOCUMENTACION/blob/main/RigthJoin.PNG"></img>	
</p>

<hr>


### Metodos SQL Server

<hr>	

> Función: ` OBTIENE LA FECHA EN LA QUE SE REALIZA LA ACCIÓN `

```md
- GETDATE(): 
```

> Función: ` COMPARA DOS FECHAS `

<hr>	

```md
- DATEDIFF(*TIPO COMPARACION*, *FECHA INICIAL*, *FECHA FINAL*): 
```

<hr>	

> Función: ` AGRUPA POR CONDITION `

```md
- GROUP BY: 
```

<hr>	

> Función: ` ORDENA POR CONDITION `

```md
- ORDER BY: 
```

<hr>	

> Función: ` SUMA VALORES `


```md
- SUM(): 
```

<hr>	

> Función: ` PROMEDIO DE VALORES `

```md
- AVG(): 
```

<hr>	

> Función: `EL VALOR MÁS GRANDE `

```md
- MAX(): 
```

<hr>	

> Función: `EL VALOR MÁS PEQUEÑO `

```md
- MIN(): 
```

<hr>	

> Función: ` CONVIERTE EN MAYUSCULAS `

```md
- UCASE(): 
```

<hr>	

> Función: `CONVIERTE EN MINUSCULAS `

```md
- LCASE(): 
```

<hr>	

> Función: `DEVUELVE LA LONGITUD DE CARACTERES DEL CAMPO `

```md
- LEN(): 
```

<hr>	

> Función: `DEVUELVE LA HORA Y FECHA ACTUALES DEL SISTEMA `

```md
- NOW(): 
```

<hr>	

> Función: ` EXTRAE CARACTERES DE UN CAMPO TEXTO`

```md
- MID(*COLUMN*, *INICIO*, *LONGITUD*):
```

<hr>	

> Función: ` CONVIERTE UN STRING EN SU REVERSO Y RETORNA EL RESULTADO `

```md
- REVERSE(): 
```

<hr>	

> Función: ` RETORNA LOS ESPACIOS DE UNA CADENA `

```md
- SPACE(): 
```

<hr>	

> Función: ` EXTRAE CARACTERES Y LO CONVIERTE UNA SUBCADENA `

```md
- SUBSTRING(): 
```

<hr>	

> Función: ` QUITA LOS ESPACIOS DE UNA CADENA `

```md
- TRIM():
```

</p>

