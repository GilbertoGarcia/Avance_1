# DISTRIBUIDORA DE AGUA EMBOTELLADA CORAL

![Base 1](https://github.com/GilbertoGarcia/Distribuidora-de-Agua-Embotellada-Coral/blob/master/Producto%20base%201.1.png)

## INTRODUCCION

Las bases de datos es un conjunto de datos pertenecientes a un mismo contexto y almacenados sistemáticamente para su posterior uso; 
esto le permite a las empresas tener un mejor control de los datos que se manejan, ya que les permite optimizar los procesos que ellas realizan. 

Este proyecto ha consistido en el desarrollo de una base de datos para un negocio ficticio, cuyas necesidades estarán descritas en los requerimientos, además se llevara a cabo hasta el punto únicamente del diseño de la base de datos, elaborándose en el margen de la asignatura de fundamentos de bases de datos.

#### INTRODUCCION A LA PROBLEMÁTICA

CORAL es una pequeña distribuidora de agua embotellada situada en el municipio de Mexicali, Baja California. Su funcionamiento principal es la venta y distribución de diferentes presentaciones de agua embotellada de un proveedor a diversos negocios de la localidad, como tiendas de abarrotes, fruterías, autoservicios y cooperativas. 

Con el constante incremento de clientes desde que comenzaron operaciones en el año 2017, la distribuidora CORAL se ha visto en la necesidad de solicitar la implementación de un sistema de bases de datos que controle las compras y ventas de los productos que maneja y de la información que tiene de sus clientes y proveedor.

## JUSTIFICACION

A través de los años las pequeñas empresas han ido evolucionando y transformando la manera en que operan sus principales funciones, todo con el fin de ofrecer un servicio de calidad a su cliente. 

Este proyecto se comenzó a desarrollar al determinar los aspectos deficientes en las operaciones que la distribuidora realizaba, como la elaboración  de los pedidos a sus clientes, la falta de un correcto control sobre los productos en existencia con los vendidos y un nulo registro que facilitara un conteo exacto y preciso sobre las botellas almacenadas en bodega. 

Por lo anterior, se justifica la necesidad de la implementación de una base de datos que pueda hacer accesible la información relacionada con la distribuidora, desde cualquier lugar y hora que sea requerido.

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

## MODELO ENTIDAD-RELACION

### REQUERIMIENTOS

En la distribución que maneja la empresa CORAL existen procesos que tienen como meta en común producir la venta de agua embotellada. Cada uno de estos procesos es cuidadosamente realizado, debido a que la incorrecta manipulación de los productos puede perjudicar al cliente y por consecuencia al negocio.

Actualmente se considera a un único proveedor, ya que por el momento brinda los productos con la calidad que los clientes demandan, pero es importante crear un apartado en la base de datos que registre la información necesaria de tal, como una clave de proveedor, nombre de la empresa, teléfono y sucursal (Ciudad, colonia, calle, número exterior).

Una vez obtenido el producto, este debe ser registrado con la siguiente información: clave de producto, nombre de producto, descripción, el costo de adquisición, cantidad y posteriormente el precio de venta. 

Se debe considerar el almacén en el que se organiza el guardado de las botellas de agua, ya que todo producto es considerado de entrada y salida, por lo que no se mantienen mucho tiempo en ella, es por eso que es importante asignarle una clave de identificación para que puedan llevar el control del saldo y merma de los productos que almacenan.

Para el proceso de ventas se debe tener registrada la información de cada uno de los clientes, como una clave que lo identifique, nombre completo, dirección (ciudad, colonia, calle, número exterior), teléfono, rfc.  Posteriormente las compras que se realicen deberán poseer una clave de compra, fecha, el nombre del cliente, producto, cantidad y concepto. 

Los registros de cada compra avalaran la existencia de una factura. Un cliente podrá poseer varias facturas, pero cada compra solo podrá ser acreedora a una única factura que consta de atributos con valor fiscal, como  una clave, rfc del cliente, notas de venta, producto vendido, cantidad vendida, descripción del producto y total a pagar.

### DIAGRAMA
![E-R](https://github.com/GilbertoGarcia/Distribuidora-de-Agua-Embotellada-Coral/blob/master/Diagrama%20Entidad%20Relacion%202.png)

### DICCIONARIO DE DATOS CONSIDERANDO LAS ENTIDADES IDENTIFICADAS
![DICCIONARIO 1](https://github.com/GilbertoGarcia/Distribuidora-de-Agua-Embotellada-Coral/blob/master/Diccionario%201%20-%20Entidades.png)

### DICCIONARIO DE DATOS CONSIDERANDO LAS RELACIONES ENTRE LAS TABLAS
![DICCIONARIO 2](https://github.com/GilbertoGarcia/Distribuidora-de-Agua-Embotellada-Coral/blob/master/Diccionario%202%20-%20Relaciones.png)

### DICCIONARIO DE DATOS CONSIDERANDO LOS ATRIBUTOS DE CADA UNA DE LAS ENTIDADES IDENTIFICADAS
![DICCIONARIO 3](https://github.com/GilbertoGarcia/Distribuidora-de-Agua-Embotellada-Coral/blob/master/Diccionario%203%20-%20Atributos.png)

## MODELO RELACIONAL
![RELACIONAL](https://github.com/GilbertoGarcia/Distribuidora-de-Agua-Embotellada-Coral/blob/master/Modelo%20Relacional.png)

![Base 2](https://github.com/GilbertoGarcia/Distribuidora-de-Agua-Embotellada-Coral/blob/master/Producto%20base%202.png)
