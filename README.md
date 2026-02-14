# taller Base de datos 

## Cristhian Andrey Padilla 

<hr>

## MODELO CONCEPTUAL

<img width="1263" height="797" alt="image" src="https://github.com/user-attachments/assets/cc256515-5376-4459-9f33-ee79bb152ba5" />

## MODELO LÓGICO 

<img width="1263" height="797" alt="image" src="https://github.com/user-attachments/assets/9a01bb19-9dd0-4796-ac71-a41c73c08fbd" />

<hr>

## Tabla 

### -Tabla Cliente

<img width="938" height="560" alt="image" src="https://github.com/user-attachments/assets/66e773d2-b365-43c6-b902-19ee899bee18" />

### -Tabla Detalle Ventas

<img width="938" height="560" alt="image" src="https://github.com/user-attachments/assets/0090110e-901c-4b22-9504-8d233c651177" />

### -Tabla Productos

<img width="938" height="560" alt="image" src="https://github.com/user-attachments/assets/2941d2ed-2446-4f91-b472-a93879ecdde4" />


### -Tabla Ventas

<img width="938" height="560" alt="image" src="https://github.com/user-attachments/assets/429a4e40-c05d-47d0-b918-cc6fa1a570b0" />

<hr>

##  Consultas 

### 1.Información del producto vendido.

```bash
SELECT producto.nombre, producto.marca, detalle_venta.cantidad, detalle_venta.subtotal
FROM producto INNER JOIN detalle_venta ON detalle_venta.id_producto = producto.id_producto
```

<img width="955" height="586" alt="image" src="https://github.com/user-attachments/assets/d5ab1daa-dfbf-408b-acdc-bac86c7ab43d" />

### 2. Cliente que han realizados ventas.

```bash
SELECT cliente.nombre, cliente.correo, venta.fecha, venta.total
FROM cliente INNER JOIN venta ON venta.id_cliente = cliente.id_cliente
```

<img width="955" height="586" alt="image" src="https://github.com/user-attachments/assets/f191fbf5-e22a-4f88-aae3-32eeb5d2b59a" />


### 3.Listar productos donde el precio este entre 50.000 y 800.000.

```bash
SELECT id_producto, nombre, marca, precio FROM producto
WHERE precio BETWEEN 50000 AND 800000 ORDER BY (precio) DESC;
```

<img width="955" height="586" alt="image" src="https://github.com/user-attachments/assets/2af92073-25ee-43ba-a1f4-5bcb6239d6be" />













