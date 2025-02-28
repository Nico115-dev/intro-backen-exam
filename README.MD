# Diseño de Base de Datos 🚀

Este repositorio contiene el diseño de una base de datos relacional para la gestión de vehículos, ventas y mantenimiento.  

## 📌 Contenido del Proyecto

1. **Diagrama UML E-R**  
   - Un diagrama con entidades, atributos y relaciones.  
   - De click para ver: [Ver Diagrama UML E-R](TU_LINK_AQUI)

2. **Documentación**  

### 📖 Documentación del Diseño de Base de Datos

#### 1. Introducción

Este documento describe el diseño de una base de datos para la gestión de un concesionario de vehículos. La base de datos almacena información sobre clientes, vehículos, ventas, servicios, mantenimiento e inventario, asegurando la integridad de los datos y la eficiencia en las consultas.

#### 2. Modelo de Base de Datos

Se ha diseñado un modelo relacional con las siguientes entidades principales:

- **Clientes:** Contiene los datos personales de los clientes.
- **Vehículos:** Almacena información sobre los automóviles, incluyendo marca, modelo, año, tipo de transmisión y combustible.
- **Vendedores:** Registra a los empleados que gestionan las ventas.
- **Ventas:** Registra las transacciones de compra realizadas por los clientes.
- **Detalle de Venta:** Relaciona las ventas con los vehículos adquiridos.
- **Tipo de Pago:** Define los métodos de pago aceptados.
- **Servicios:** Almacena los servicios realizados a los vehículos.
- **Tipo de Servicio:** Clasifica los servicios disponibles.
- **Mantenimiento:** Registra detalles sobre mantenimientos realizados a los vehículos.
- **Orden de Mantenimiento:** Relaciona clientes con mantenimientos realizados.
- **Inventario:** Controla la disponibilidad de vehículos en los concesionarios.
- **Concesionario:** Contiene información de las sucursales.
- **Tipo de Transmisión:** Define las transmisiones disponibles.
- **Tipo de Combustible:** Define los tipos de combustible usados.

#### 3. Justificación de las Relaciones

El diseño está basado en relaciones 1 a muchos (1:N) y 1 a 1 (1:1), evitando relaciones muchos a muchos (N:M). Las principales relaciones son:

- **Un cliente puede tener varios vehículos, pero un vehículo pertenece a un solo cliente.**
- **Una venta es realizada por un cliente y gestionada por un vendedor.**
- **Cada venta puede incluir varios vehículos, pero cada vehículo en la venta pertenece a una sola transacción.**
- **Un vehículo puede recibir varios servicios, pero cada servicio está vinculado a un solo vehículo.**
- **El mantenimiento está relacionado con un servicio específico.**
- **Un cliente puede generar varias órdenes de mantenimiento.**
- **El inventario almacena vehículos en un concesionario específico.**

#### 4. Restricciones y Consideraciones

- Se establecen claves primarias en todas las tablas.
- Se utilizan claves foráneas para mantener la integridad referencial.
- Se evita la redundancia de datos mediante la normalización.
- Se agregan restricciones como `"NOT NULL"` para garantizar la consistencia de los datos.

#### 5. Conclusión

El diseño de la base de datos permite una gestión eficiente de los datos del concesionario, asegurando la integridad y optimización de consultas. Su estructura está preparada para escalar y adaptarse a futuras mejoras o integraciones.

3. **SQL Script**  
   - Un script SQL que crea las tablas y restricciones necesarias para la base de datos.
   - De click para ver: [Ver SQL Script](TU_LINK_AQUI)

