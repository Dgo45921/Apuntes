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
 En particular, los sistemas que se encuentran en máquinas grandes ( s i s
temas grandes") tienden a ser multiusuario, mientras que los que se ejecutan en máquinas pe
queñas ("sistemas pequeños") tienden a ser de un solo usuario. Un sistema de un solo usuario
es aquel en el que sólo un usuario puede tener acceso a la base de datos en un momento dado;
un sistema multiusuario es aquel en el cual múltiples usuarios pueden tener acceso simultáneo
a la base de datos.
**Los datos en una base de datos son tanto integrados como compartidos**

# Integrados 
implica una base de datos de varios archivos unificados, con redundancia pre-eliminada 

# Coompartidos
Simplemente se refiere al acceso por medio completo de los usuarios al *MISMO TIEMPO*

# Concurrencia 
Puede soportar multiples consultas

Si la **Base de Datos** es compartida, entonces es *Base de datos personal* esto implica la secuencia física de redes *SAN* con *RAID* del 1 al 5. 

## Hardware en Bases de Datos
Los componentes principales tiended a ser: 
*1. Volumenes de Almacenamiento Secundario* Estos tienden a ser *DISCOS MAGNETICOS* para
contender datos almacenados, junto con dispositivos I/O. 
Específicamente, en clase se hizo énfasis en este tema: 
- Depende de la configuración de las conexiones por medio de un Balanceo de Cargas
- Específicamente depende de las llaves primarias eficientes (Evitar tipo caracter)

*2. Procesadores de Hardware y Memoria Principal* utilizada para apoyar la ejecución del software. 

## Software
Entre la Base de Datos física y los datos almacenados físicamente existe una capa de software. O bien
**DBMS** 
*Debe ocultar el funcionamiento, solamente se deberian mostrar los resultados utilizando queries*
| Aspectos de DBMS | 
-------------------
| Componente mas importante del sistema general. | 
| Existen otros componentes de desarrollo como el monitor PT o administrador de Transacciones | 
-----------------------------------------------------------------------------------------------

## Usuarios 
En teoria, existen 3 tipos de usuarios: 
1. Developers: Utilizaran la DBMS para realizar consultas
2. Usuarios Finales: Interactuan desde estaciones de trabajo o terminales en linea.
3. DBA (Database Administrator): Demás

# ¿Qué es una Base de Datos? 
- Datos persistentes (Operacionales o de Producción)
■ Una base de datos es un conjunto de datos persistentes que es utilizado por los sistemas de
aplicación de alguna empresa dada.

## Entidades y Relaciones 
### Entidades
El término *entidad* es
empleado comúnmente en los círculos de bases de datos para referirse a cualquier objeto distinguible que va a ser representado en la base de dato. 

### Vinculos 
Responde a la pregunta ¿Como se asocian dichas basicas?
![image](https://github.com/Dgo45921/Apuntes/assets/79114580/95c44d37-8ac9-4744-9363-09c5e4499a5f)

Aunque la mayoría de los vínculos de la figura comprenden dos tipos de entidad (es decir.
son vínculos binarios) no significa que todos los vínculos deban ser necesariamente bina
rios en este aspecto
#### Propiedades 
Las entidades poseen propiedades que corresponded a la información que desamos registrar sobre ellas. 
Estas "Propiedades" también pueden ser llamadas "atributos"

#### Datos y Modelos de Datos
## Datos 
Se deriva del latín "Dar" en realidad, son hechos dados. Una colecciones de tales proposiciones verdaderas. 
## Modelo de Bases de Datos Relacional 
En este modelo se pueden identificar distintas cosas: 
- Tablas, los datos son filas y las filas pueden ser interpretadas como proposiciones verdaderas
- Se proporcionan operadores para operar sobre las columnas de las tablas, estos operadores
- sopertan directamente el proceso de inferir proposiciones verdaderas. 

Sin embargo, el modelo relacional no es el unico.

## Modelo de Datos 
Es una definicion lofica, independiete y abstracta de los objetos operadores y demas conjuntos que contiruyen una maquina abstracta con la que interactuan lo usuarios. 
Los operadores modelan el comportamiento de ellos. Los objetos permiten modelar.

**El modelo es aquello que los usuarios tienen que conocer; la implementación es
lo que los usuarios no tienen que conocer.**
Los modelos pueden ser *Logicos* y *Fisicos*. Sin emabrgo, muchos de las bases de datos actualmente no hacen esas diferencias. 
■ En el primer sentido, un modelo de datos es como un lenguaje de programación (aunque
en cierto modo abstracto) cuyos elementos pueden ser usados para resolver una amplia va
riedad de problemas específicos, pero que en sí y por sí mismos no tienen una conexión di
recta con ninguno de estos problemas específicos.
■ En el segundo sentido, un modelo de datos es como un programa específico escrito en ese
lenguaje. En otras palabras, un modelo de datos que toma las características que ofrece al
gún modelo como el primero y las aplica a cierto problema específico. Puede ser visto como
una aplicación específica de algún modelo con el primer significado

# ¿Por qué una base de datos?  
## Beneficios de un solo usuario 
![image](https://github.com/Dgo45921/Apuntes/assets/79114580/6094a3c5-daa1-4060-be4a-c8a8033e644e)
El sistema de base de datos ofrece a la empresa un control centralizado de sus
datos (los cuales, como se habrá dado cuenta a estas alturas, constituyen uno de sus activos más
valiosos). 
# Administrador de Bases de Datos y Administrador de datos
El *Administrador de Datos* es la persona que tiene responsabilidad central sobre los datos. 
Ya que (repitiendo) los datos son uno de los activos más valiosos de la
empresa, es imperativo que exista una persona que los entienda junto con las necesidades de
la empresa con respecto a esos datos, a un nivel de administración superior. Esa persona es
el administrador de datos. 
![image](https://github.com/Dgo45921/Apuntes/assets/79114580/2f86cb18-5601-4f9d-8b40-aea286cb14ec)
## Beneficios del enfoque de datos
- Los datos pueden compartirse
- Es posible reducir la redundancia
- Brindar un manejo de Transacciones
una **Transaccion** es una unidad de trabajo lógica, que por lo regultar comprende varias operaciones de la base de datos.
La **Atomicidad** de las transacciones se refiere a poder completar o no las transacciones. Por ejemplo, si la transaccion se queda a medias, esta puede ser revertida y el estado actual de la DB se muestra normal. 
- Integridad
  El problema de la integridad es el de asegurar que los datos de la base de datos estén correctos.
  El **DBA** debe implementar restricciones de integridad (o Reglas del negocio)
  ![image](https://github.com/Dgo45921/Apuntes/assets/79114580/9b50c778-2d24-4158-a699-a1bb3f4b5c01)

- Es posible hacer cumplir la seguridad
  EL DBA oyede asegurar que el unico medio de acceso a la base de datos sea a traves de los canales adecuados y por lo tanto puede definir las reglas o restricciones de seguridad.
- Es posible equilibrar los requerimientos en conflicto
  Al conocer los requerimientos generales de la empresa (a diferencia de los requerimientos
de los usuarios individuales), el DBA puede estructurar los sistemas de manera que ofrezcan un servicio general que sea "el mejor para la empresa" (de nuevo bajo la dirección del
administrador de datos).
- Es posible hacer cumplir los estandares
  Con el control central de la base de datos, el DBA (una vez más, bajo la dirección del administrador de datos) puede asegurar que todos los estándares aplicables en la representación de los datos sean observados. Estos estándares podrían incluir alguno o todos los
siguientes: departamentales, de instalación, corporativos, de la industria, nacionales e internacionales.
  
Recordar que las caracteristicas principales son
**ATOMICIDAD**, **AISLAMIENTO**, **DURABILIDAD**, **CONSISTENCIA**
  ![image](https://github.com/Dgo45921/Apuntes/assets/79114580/7e0a5fd9-344a-4a99-bb26-4524c53ef0b9)

Podemos inferir entonces que
# No Redundancia -> Inconsistencia -> No integro

# Independencia de Datos 
Existen 2 tipos de independencia de datos: *Fisica* y *Logica*
Basicamente la dependencia fisica de datos se refiere a la estricta dependencia de los datos sobre otros. En el caso de los modelos entidad-relacion, implica que los datos dependen de otros en otras tablas. 
x
### Terminos importantes sobre arquitecturas de DB 
#### Campo almacenado 
La unidad mas pequeña de datos almacenados. Este contiene **Ocurrencias** De diversos **Tipos** de campos almacenados. 
Una ocurrencia (o ejemplar) de registro almacenado consta de un grupo de ocurrencias de campos almacenados relacionados. Por ejemplo,
una ocurrencia de registro almacenado dentro de la base de datos "partes" podría consistir
en una ocurrencia de cada uno de los siguientes campos almacenados: número de parte,
nombre de parte, color de parte y peso de parte. Decimos que la base de datos contiene muchas ocurrencias del tipo de registro almacenado "parte" (una vez más, una ocurrencia por
cada clase de parte).
Textualmente el libro dice
'''
Una ocurrencia (o ejemplar) de registro almacenado consta de un grupo de ocurrencias de campos almacenados relacionados. Por ejemplo,
una ocurrencia de registro almacenado dentro de la base de datos "partes" podría consistir
en una ocurrencia de cada uno de los siguientes campos almacenados: número de parte,
nombre de parte, color de parte y peso de parte. Decimos que la base de datos contiene muchas ocurrencias del tipo de registro almacenado "parte" (una vez más, una ocurrencia por
cada clase de parte).

Por último, un archivo almacenado es la colección de todas las ocurrencias existentes actualmente para un tipo de registro almacenado. Nota: Por simplicidad damos por hecho que
todo archivo almacenado contiene sólo un tipo de registro almacenado. Esta simplificación
no afecta sustancialmente ninguna de las explicaciones subsecuentes.
''' 
## Representacion de Datos 
### Datos numericos
Formas aritmeticas internas o como una cadena de caracteres. 
### Datos de Caraacteres 
Mentiante ASCII, EBCDIC o Unicode. 
### Unidades para datos numericos 
Las unidades en un campo numerico puede cambiar con el tiempo
### Codificacion de los datos 
En ciertas situaciones, podria ser conveniente representar los datos almacenados por medio de valores codificados. 
### Materializacion de los datos 
En la practica, el campo logico
![image](https://github.com/Dgo45921/Apuntes/assets/79114580/9bf0dca1-5652-4514-b726-ffbc55149946)
NOTA> SE DEBE COMPLETAR CON EL EJEMPLO PRACTICO DEL LIBRO 

# Sistemas Relacionales y Otros Sistemas
Los DBMS que se basan en el modelo relacional. 
## ¿ Qué es un sistema relacional? 
Un sistema en el cual los datos son percibidos como tablas y los operadores disponibles para el usuario son operadores que generan nuevas tablas a partir de las anteriores. 
NOTA> SE DEBE COMPLETAR CON EL EJEMPLO PRACTICO DEL LIBRO 
# Lenguajes en Bases de Datos
## DDL 
Data Definition Languages: Permite la definicion o declaracion de objetos de bases de datos. 
Incluso pueden existir híbridos entre DCL y demás. 
## DML 
Data Manipulation Language: permite la manupulacion o procesamiento de dichos objetos. 

# Productos Relacionales
Los primeros productos relacionales operan en los años 70. 

# Resumen general 
Cerramos este capítulo introductorio con un resumen de las ideas principales expuestas. Primero,
es posible pensar en un sistema de base de datos como un sistema de registros computarizado.
Dicho sistema comprende a los propios datos (almacenados en la base de datos), al hardware, al
software (en particular al sistema de administración de base de datos o DBMS) y (¡lo más
importante!) a los usuarios. A su vez, los usuarios pueden ser divididos en programadores de
aplicaciones, usuarios finales y administrador de base de datos o DBA. El DBA es el responsable de administrar la base de datos y el sistema de base de datos, de acuerdo con las políticas
establecidas por el administrador de datos.
Las bases de datos están integradas y por lo regular son compartidas; se emplean para almacenar datos persistentes. Dichos datos pueden considerarse, de manera útil aunque informal,
como una representación de entidades, junto con los vínculos que están entre éstas (aunque de
hecho, un vínculo es en realidad sólo una clase especial de entidad). Analizaremos brevemente
la idea de los diagramas de entidad/vínculo
