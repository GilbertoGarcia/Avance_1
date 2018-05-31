# DISTRIBUIDORA DE AGUA EMBOTELLADA CORAL

![Base 1](https://github.com/GilbertoGarcia/Distribuidora-Agua-Embotellada-Coral/blob/master/Material%20Visual/Cabecera%201.png)

## INTRODUCCION

Las bases de datos son un conjunto de datos pertenecientes a un mismo contexto, almacenados sistemáticamente para su posterior uso, permitiendo a las empresas tener un mejor control de los datos que se manejan, ya que les permite optimizar los procesos que ellas realizan. 

Este proyecto ha consistido en el desarrollo de una base de datos para un negocio ficticio, cuyas necesidades estarán descritas en los requerimientos, además se llevara a cabo hasta el punto de implementarlo en MySQL, labor que se encuentra al margen de la asignatura de fundamentos de bases de datos.

#### PROBLEMÁTICA

**CORAL** es una pequeña distribuidora de agua embotellada situada en el municipio de Mexicali, Baja California. Su funcionamiento principal es la venta y distribución de diferentes presentaciones de agua embotellada de varios proveedores a diversos negocios de la localidad, como tiendas de abarrotes, fruterías, autoservicios y cooperativas. 

Con el constante incremento de clientes desde el comienzo de operaciones en el año 2017, la distribuidora CORAL ha determinado aspectos deficientes en las operaciones que realiza, como la pobre elaboración  de los pedidos de sus clientes, la falta de un correcto control sobre los productos en existencia con respecto a los vendidos y un nulo registro que facilite un conteo exacto y preciso sobre las botellas almacenadas en bodega, por ende se ha visto en la necesidad de solicitar la implementación de un sistema de bases de datos que controle los pedidos de los productos que maneja y la información de sus clientes y proveedores.

## JUSTIFICACION

A través de los años las pequeñas empresas han ido evolucionando y transformando la manera en que operan sus principales funciones, todo con el fin de ofrecer un servicio de calidad a su cliente. 

Es por esto que se justifica la necesidad de la implementación de una base de datos que pueda hacer accesible la información relacionada con la distribuidora, desde cualquier lugar y hora que sea requerido.

## OBJETIVO GENERAL

Desarrollar una base de datos para el control de compras, clientes y registro de almacenaje de las diferentes presentaciones de agua embotellada que la Distribuidora CORAL maneja.

### OBJETIVOS ESPECIFICOS

**1.	Facilitar una mejor forma de organización de la información que relaciona a la distribuidora.**

**2.	Elaborar una base de datos que pueda desplegar un reporte útil de las diferentes áreas de la distribuidora para la toma de decisiones.**

**3.	Se podrá consultar, ingresar y modificar los datos de todas las operaciones de la distribuidora.**

**4.	Agilizar los procesos de compras, tanto en el estado de recibir los pedidos como en la facturación del mismo.**

**5.	Proporcionar persistencia a la base de datos a medida que se desarrolla para el cliente.**

**6.	A pesar de que el desarrollo de este proyecto será al margen de la asignatura de Fundamentos de Bases de datos esta debe pensarse en permitir a la interface en medida a ignorar la estructura interna de la Base de Datos.**

**7.	Proporcionar la documentación que describa la estructura de la Base de Datos y sus procedimientos.**

**8.	La Base de Datos deberá cumplir con los requerimientos establecidos.**

**9.	La Base de Datos debe ser escalable, permitiendo la incorporación progresiva de nuevas funcionalidades.**

**10.	Definir dinámicamente entidades y atributos adicionales para gestionar la información de referencia.**

**11.	Utilizar las herramientas de MySQL para la implementación de la base de datos.**

## MODELO ENTIDAD-RELACION

### REQUERIMIENTOS

En la distribución que maneja la empresa CORAL existen procesos que tienen como meta en común producir la venta de agua embotellada. Cada uno de estos procesos es cuidadosamente realizado, debido a que la incorrecta manipulación de los productos puede perjudicar al cliente y por consecuencia al negocio.

Se consideran los proveedores, porque brindan los productos con la calidad que los clientes demandan, por eso es importante crear un apartado en la base de datos que registre la información necesaria de tales, como una clave de proveedor, nombre de la empresa, teléfono y sucursal (Ciudad, colonia, calle, número de zona).

Una vez obtenido el producto, este debe ser registrado con la siguiente información: clave de producto, nombre de producto, descripción, el costo de adquisición, cantidad y posteriormente el precio de venta. 

También se debe considerar el almacén en el que se organiza el guardado de las botellas de agua, ya que todo producto es considerado de entrada y salida, por lo que no se mantienen mucho tiempo en ella, es por eso que es importante asignarle una clave de identificación para que puedan llevar el control del saldo y merma de los productos que almacenan.

Para el proceso de pedidos se debe tener registrada la información de cada uno de los clientes, como una clave que lo identifique, nombre completo, dirección (ciudad, colonia, calle, número de zona), teléfono, rfc. Posteriormente los pedidos que se realicen deberán poseer una clave de pedido, fecha, el nombre del cliente, producto, cantidad y concepto.

Los registros de cada pedido avalarán la existencia de una factura. Un cliente podrá poseer varias facturas, pero cada pedido sólo podrá ser acreedora a una única factura que consta de atributos con valor fiscal, como  una clave de factura, rfc del cliente, notas de venta, producto vendido, cantidad vendida, descripción del producto y total a pagar. 

### DIAGRAMA
![E-R](https://github.com/GilbertoGarcia/Distribuidora-Agua-Embotellada-Coral/blob/master/Material%20Visual/Diagrama%20Entidad%20Relacion.png)

### DICCIONARIO DE DATOS CONSIDERANDO LAS ENTIDADES IDENTIFICADAS
![DICCIONARIO 1](https://github.com/GilbertoGarcia/Distribuidora-Agua-Embotellada-Coral/blob/master/Material%20Visual/Diccionario%201%20-%20Entidades.png)

### DICCIONARIO DE DATOS CONSIDERANDO LAS RELACIONES ENTRE LAS TABLAS
![DICCIONARIO 2](https://github.com/GilbertoGarcia/Distribuidora-Agua-Embotellada-Coral/blob/master/Material%20Visual/Diccionario%202%20-%20Relaciones.png)

### DICCIONARIO DE DATOS CONSIDERANDO LOS ATRIBUTOS DE CADA UNA DE LAS ENTIDADES IDENTIFICADAS
![DICCIONARIO 3](https://github.com/GilbertoGarcia/Distribuidora-Agua-Embotellada-Coral/blob/master/Material%20Visual/Diccionario%203%20-%20Atributos%20Base.png)

### REDES SEMANTICAS

![SEM 1](https://github.com/GilbertoGarcia/Distribuidora-Agua-Embotellada-Coral/blob/master/Material%20Visual/Red%201.png)
![SEM 2](https://github.com/GilbertoGarcia/Distribuidora-Agua-Embotellada-Coral/blob/master/Material%20Visual/Red%202.png)
![SEM 3](https://github.com/GilbertoGarcia/Distribuidora-Agua-Embotellada-Coral/blob/master/Material%20Visual/Red%203.2.png)
![SEM 4](https://github.com/GilbertoGarcia/Distribuidora-Agua-Embotellada-Coral/blob/master/Material%20Visual/Red%203.1%20Productos.png)

## MODELO RELACIONAL
![RELACIONAL](https://github.com/GilbertoGarcia/Distribuidora-Agua-Embotellada-Coral/blob/master/Material%20Visual/Modelo%20Relacional%20Base.png)

![Base 2](https://github.com/GilbertoGarcia/Distribuidora-Agua-Embotellada-Coral/blob/master/Material%20Visual/Cabecera%202.png)
