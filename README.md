# GdD-2022-2C
Trabajo Practico de Gestion de Datos | 2C 2022 

Prof: Edgardo Luis Lacquaniti 

Grupo: Matias Argonz, Camila Andrea Berro, Juan Alberto Flores Maquera.


El trabajo práctico consiste en implementar un nuevo sistema que se encargue de la
gestión de un negocio que vende artículos de un Bazar. Se registra la información de ventas
y compras de productos, información de compradores y proveedores, y a su vez información
de productos en específico.

En algunas tablas, se propuso usar un id autoincremental para que sea más sencillo
identificar la entidad. Por ejemplo, en la tabla Proveedor se usó este tipo de PK ya que sino
se tendría que identificar usando 2 pks diferentes(proveedor_razon_social, proveedor_cuit).
Las funciones creadas que se usan en migración son de utilidad para obtener los id
correspondientes a través de los campos conocidos que fueron provistos por la cátedra en
la tabla maestra.

Se decidió usar una tabla llamada CompraXProducto como intermedia de la tabla
compra y producto_variante (se hizo lo mismo en VentaXProducto para producto_variante y
venta) para que exista la relación entre las dos tablas. En ambas tablas se decidió usar un
pk autoincremental ya que el código de la compra/venta de un producto y el producto
variante código se encontraba repetido en un dato, con la diferencia que la cantidad
comprada era diferente.

Se decidió para el esquema del modelo, crear las tablas correspondientes por un
lado y por otro las PKs y Fks de ellas. De esta manera, no dependemos del orden en el que
se ejecuta la creación de las tablas.
Por último, la duración promedio de la migración es de aproximadamente 3 minutos
y 8 segundos, dependiendo de la computadora usada.
