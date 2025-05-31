# Caso de Uso: Repetir Pedidos

### Versión
1.0

### Fecha
5/31/2025

### Autores
Joel Rillo Fernández

---

### Descripción
Los clientes pueden repetir pedidos desde su historial.

---

### Actores
- Cliente  

---

### Precondiciones
El usuario debe estar registrado y estar viendo su historial de pedidos.

---

### Flujo Principal
1. El cliente elige un pedido dentro de su historial.
2. El pedido se vuelve a realizar con los mismos detalles que cuando se realizo por primera vez.

---

### Flujos Alternativos
- **Uno o mas de los platos que forman el pedido deseado ya no está disponible.** 
  Un pop-up avisará al cliente de la situación y listará los platos no disponibles. A partir de este pop-up el cliente puede elegir si continuar sin dichos platos o si cancelar el pedido.
- **El usuario ya tiene tres pedidos activos.**
  Un pop-up avisará al cliente y le impedirá realizar el pedido.
  
---

### Postcondiciones
El pedido se envía al mismo cocinero que lo cocinó la vez anterior.

---

### Requisitos No Funcionales
- Pedidos sólo para usuarios registrados.
- Restricción de pedidos.

---

### Prioridad
Baja.
