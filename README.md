# Consulta #1 Sql

## CONSULTAS SQL


1. Para visualizar toda la información que contiene la tabla `usuario` se puede incluir con la instrucción SELECT el caracter `*` o cada una de los campos de la tabla 

`SELECT * FROM usuario`

![Consulta-1](img/1.png "Tabla usuario")

2. Seleccionar o visualizar solamente la identificación del usuario.

`SELECT Identificación FROM usuario`

![Consulta-2](img/2.png "Tabla Identificacion")

3. Si se desea obtener los registros cuya identificacion sean mayores o iguales a 150, se debe utilizar la consulta WHERE que especifica las condiciones que deben reunir los registros que se van a seleccionar-

`SELECT * FROM usuario WHERE identificacion >= 150`

![Consulta-3](img/tabla_mayorque.png "Tabla Mayor o igual que")

4. Si se desea obtener los registros cuyo sus apellidos sean Vanegas o Cetina, se debe utilizar el operador IN que especifica los registros 
`SELECT apellidos FROM usuario WHERE apellidos IN ('Vanegas', 'Cetina')`

![Consulta-4](img/tabla_apellidos1.png "Tabla Apellidos1")

### O se puede utilizar el operador OR.

`SELECT apellidos FROM usuario WHERE apellidos='Vanegas' OR apellidos='Cetina'`

![Consulta-4.1](img/tabla_apellidos2.png "Tabla Apellidos2")

5. Si se desea obtener los registros cuya identificacion sea menor de '110' y la ciudad sea 'Cali', se debe utilizar el operador AND.

`SELECT * FROM usuario WHERE identificacion < 110 AND ciudad_nac='Cali'`

![Consulta-5](img/tabla_iden-ciudad.png "Tabla Apellidos2")

6. Si se desa obtener los registros cuyos nombres empiecen por la letra a, sebe utilizar l operador LIKE que utiliza los patrones "%" (todos) y '_' (caracter)

`select * from Usuario where nombre LIKE 'A%'`

![Consulta-6](img/7.png "Consulta 6")

7. Se desea obtener los registros cuyos nombres tengan la letra a

`select * from Usuario where nombre LIKE '%a%'`

![Consulta-7](img/8.png "Consulta 7")


