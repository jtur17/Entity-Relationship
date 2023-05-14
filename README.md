# Entity Relationship

Lo que he hecho ha sido diseñar una base de datos que permita almacenar la información de los datos de un concesionario de coches.

Los clientes tiene 3 atributos que son DNI que es la clave principal, el nombre y el teléfono en la que tiene una relación muchos a muchos con empleado en el que tiene 5 atributos que son Nombre, Dirección, ID_Empleado, Correo y Teléfono. Además le asignamos un rol recursivo que se llama jefe en la que puede ser Supervisor o supervisado 

La tabla de empleado tiene una relacion de 1 a muchos con vehículo en la que tiene 4 atributos, Matricula que es la clave principal, Modelo, Color y precio. También tiene una especialización total en la que el vehículo solo puede ser o Moto o Coche, si es una moto tiene 2 atributos que son Cilindrada, Tipo de moto y si es coche tiene otros dos atributos que son Puertas y Tipo de coche. Luego vehículo tiene una entidad debil de 1 a muchos en el que tiene una dependiente que se llama Número de Airbags.

Clientes tambien tiene una relación de 1 a muchos con vehiculos en el que la relación tiene un atributo que es fecha de compra.