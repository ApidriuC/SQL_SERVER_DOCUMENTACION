<h1 align="center">DOCUMENTACIÓN SQL SERVER</h1>

<p align="justify">

### Usar una base de datos específica	
	
```md
USE *DB*
```

<hr>

### Crear Base de Datos
```md
Create Data Base *Nombre*
```

<hr>

### Crear una nueva tabla

```md
CREATE TABLE *DATABASE NAME* (
	PK_1 DATA TYPE PRIMARY KEY IDENTITY NOT NULL,
	COLUMN_1 DATA TYPE NOT,
	FK_1
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

### Joins entre tablas
```md
SELECT *
FROM *TABLE*
*TYPE JOIN* JOIN *TABLE* AS *PSUDONAME* ON *CONDITION JOIN*
WHERE *CONDITION SELECT*
```

<hr>

### Metodos SQL Server

> Función: ` OBTIENE LA FECHA EN LA QUE SE REALIZA LA ACCIÓN `

```md
- GETDATE(): 
```

> Función: ` COMPARA DOS FECHAS `

```md
- DATEDIFF(*TIPO COMPARACION*, *FECHA INICIAL*, *FECHA FINAL*): 
```

> Función: ` AGRUPA POR CONDITION `

```md
- GROUP BY: 
```

> Función: ` ORDENA POR CONDITION `

```md
- ORDER BY: 
```

> Función: ` SUMA VALORES `


```md
- SUM(): 
```

> Función: ` PROMEDIO DE VALORES `

```md
- AVG(): 
```

> Función: `EL VALOR MÁS GRANDE `

```md
- MAX(): 
```

> Función: `EL VALOR MÁS PEQUEÑO `

```md
- MIN(): 
```

> Función: ` CONVIERTE EN MAYUSCULAS `

```md
- UCASE(): 
```

> Función: `CONVIERTE EN MINUSCULAS `

```md
- LCASE(): 
```

> Función: `DEVUELVE LA LONGITUD DE CARACTERES DEL CAMPO `

```md
- LEN(): 
```

> Función: `DEVUELVE LA HORA Y FECHA ACTUALES DEL SISTEMA `

```md
- NOW(): 
```

> Función: ` EXTRAE CARACTERES DE UN CAMPO TEXTO`

```md
- MID(*COLUMN*, *INICIO*, *LONGITUD*):
```

> Función: ` CONVIERTE UN STRING EN SU REVERSO Y RETORNA EL RESULTADO `

```md
- REVERSE(): 
```

> Función: ` RETORNA LOS ESPACIOS DE UNA CADENA `

```md
- SPACE(): 
```

> Función: ` EXTRAE CARACTERES Y LO CONVIERTE UNA SUBCADENA `

```md
- SUBSTRING(): 
```

> Función: ` QUITA LOS ESPACIOS DE UNA CADENA `

```md
- TRIM():
```

</p>

