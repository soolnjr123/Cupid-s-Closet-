# Alcance del proyecto - Cupid's Closet

## 1. ¿Cuál es el problema que resuelve el sistema?

Cupid's Closet busca resolver la dificultad que tienen muchos emprendimientos de ropa para organizar y mostrar sus productos de manera clara en una tienda online.

Muchas tiendas utilizan solamente redes sociales para mostrar sus productos, lo que puede dificultar la búsqueda de prendas, la consulta de precios, la organización por categorías y la realización de pedidos.

## 2. ¿Quiénes son los usuarios?

### Cliente

El cliente podrá ingresar a la tienda, visualizar las prendas disponibles, buscar productos, utilizar filtros, agregar productos al carrito y utilizar la función "Encontrá tu outfit".

### Administrador

El administrador será la persona encargada de gestionar la tienda. Podrá agregar, modificar y eliminar productos, además de administrar precios, categorías y stock.

## 3. Funcionalidades mínimas

1. Visualizar el catálogo de productos.
2. Buscar productos por nombre.
3. Filtrar prendas por categorías.
4. Agregar productos al carrito.
5. Calcular el precio total del carrito.
6. Utilizar la función "Encontrá tu outfit".
7. Registrar pedidos.
8. Administrar productos.

## 4. Entidades de la base de datos

### Productos

- id
- nombre
- descripción
- precio
- categoría
- stock
- imagen

### Usuarios

- id
- nombre
- email
- contraseña
- tipo de usuario

### Pedidos

- id
- usuario_id
- fecha
- total
- estado

### Detalle de pedido

- id
- pedido_id
- producto_id
- cantidad
- precio

## 5. Endpoints de la API REST

GET /api/productos  
Permite obtener todos los productos.

GET /api/productos/:id  
Permite obtener un producto específico.

POST /api/productos  
Permite agregar un nuevo producto.

PUT /api/productos/:id  
Permite modificar un producto existente.

DELETE /api/productos/:id  
Permite eliminar un producto.

POST /api/pedidos  
Permite registrar un nuevo pedido.

GET /api/pedidos  
Permite consultar los pedidos registrados.

## 6. Mejoras futuras

En futuras versiones se podrían agregar:

- Inicio de sesión.
- Productos favoritos.
- Historial de compras.
- Pagos mediante Mercado Pago.
- Seguimiento de pedidos.
- Recomendaciones personalizadas.
- Aplicación móvil.