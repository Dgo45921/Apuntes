# Lectura 1 - Libro CJ Introducción a las Bases de Datos 
# Capitulo 1

**¿Qué es una Base de Datos?**
Un sistema de Bases de Datos es básicamente un sistema computarizado para mantener datos. 
Este permite la realización de las siguientes acciones:
- Agregar nuevos archivos vacios
- Insertar datos dentro de archivos existentes
- Recuperar datos de los Archivos existentes
- MOdificar datos en archivos existentes
- Eliminar datos en archivos existentes
- Eliminar archivos existentes de la Base de Datos

Básicamente son INSERCIÓN, MODIFICACIÓN y ELIMINACIÓN
```sql
-- Inserción de datos nuevos:
INSERT INTO CAVA ( NICHO#, VINO, PRODUCTOR, AÑO, BOTELLAS, LISTO )
VALUES ( 53, 'Pinot Noir', 'Sainsbury', 1997, 6, 2001 );

-- Modificación de datos existentes:
UPDATE CAVA
SET BOTELLAS = 4
WHERE NICHO# = 3;

-- Eliminación de datos existentes:
DELETE FROM CAVA
WHERE NICHO# = 2;
```
A las tablas se les llama **Relaciones**
| Término       | Descripción |
|---------------|-------------|
| Registro      | Un registro es una fila completa en una tabla de base de datos; contiene información única para un elemento específico en la tabla. |
| Fila          | Una fila es sinónimo de registro, refiriéndose a una línea horizontal en una tabla que contiene datos específicos organizados en columnas. |
| Columna       | Una columna es una estructura vertical en una tabla que contiene todos los datos de un campo específico en la base de datos. |
| Campo         | Un campo es un espacio específico en una tabla que almacena un tipo particular de dato dentro de una columna. |

## ¿Qué es un sistema de bases de datos?
Básicamente es un sistema computarizado que permite guardar registros. 
Su finalidad es almacenar información y permitir que lo susuarios
puedan recuperar y actualizar dicha información. 
![image](https://github.com/Dgo45921/Apuntes/assets/79114580/2ed790e6-9624-41f6-9965-6acf742cb06f)

## Definiciones Base
# Datos


