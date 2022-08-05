<h1 align="center">DOCUMENTACIÓN SQL SERVER</h1>

<p align="justify">

USE *DB*
---------------------------------------------------------------------------
CREATE TABLE *DATABASE NAME* (
	PK_1 DATA TYPE PRIMARY KEY IDENTITY NOT NULL,
	COLUMN_1 DATA TYPE NOT,
	FK_1
	FOREIGN KEY (*FK_1*) REFERENCES *TABLE* (*PK TABLE*) 
)
---------------------------------------------------------------------------
SELECT *
FROM *TABLE*
WHERE *CONDITION* 
---------------------------------------------------------------------------
INSERT INTO *TABLE*(*COLUMNS*) VALUES (*VALUES*)
---------------------------------------------------------------------------
UPDATE *TABLE* SET *COLUMN* = *VALUE* WHERE *CONDITION* 
---------------------------------------------------------------------------
*DELETE ROWS*
DELETE FROM *TABLE* WHERE *CONDITION*
---------------------------------------------------------------------------
*DELETE COLUMNS*
ALTER TABLE *TABLE* DROP COLUMN *COLUMN*;
---------------------------------------------------------------------------
*JOINS*
SELECT *
FROM *TABLE*
*TYPE JOIN* JOIN *TABLE* AS *PSUDONAME* ON *CONDITION JOIN*
WHERE *CONDITION SELECT*
---------------------------------------------------------------------------
*METHODS*

GETDATE(): OBTIENE LA FECHA EN LA QUE SE REALIZA LA ACCIÓN

DATEDIFF(*TIPO COMPARACION*, *FECHA INICIAL*, *FECHA FINAL*): COMPARA DOS FECHAS

GROUP BY: AGRUPA POR

ORDER BY:

SUM(): SUMA VALORES

AVG(): PROMEDIO DE VALORES

MAX(): EL VALOR MÁS GRANDE

MIN(): EL VALOR MÁS PEQUEÑO

UCASE(): CONVIERTE EN MAYUSCULAS

LCASE(): CONVIERTE EN MINUSCULAS

LEN(): DEVUELVE LA LONGITUD DE CARACTERES DEL CAMPO

NOW(): DEVUELVE LA HORA Y FECHA ACTUALES DEL SISTEMA

MID(*COLUMN*, *INICIO*, *LONGITUD*): EXTRAE CARACTERES DE UN CAMPO TEXTO

REVERSE(): CONVIERTE UN STRING EN SU REVERSO Y RETORNA EL RESULTADO

SPACE(): RETORNA LOS ESPACIOS DE UNA CADENA

SUBSTRING(): EXTRAE CARACTERES Y LO CONVIERTE UNA SUBCADENA

TRIM(): QUITA LOS ESPACIOS DE UNA CADENA
---------------------------------------------------------------------------
</p>
