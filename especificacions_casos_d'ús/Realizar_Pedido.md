# Caso de Uso: Realizar Pedido

### Versión
1.0

### Fecha
6/1/2025

### Autores
Joel Rillo Fernández

---

### Descripción
El cliente puede enviar un pedido que consta del menú seleccionados.

---

### Actores
- Cliente

---

### Precondiciones
Antes de poder realizar un primer pedido los clientes deberán llenar un pequeño perfil. En este indicarán su dirección de recogida de pedido y, opcionalmente, restricciones alimentarias (alergias, comidas que no quieren recibir) así como definir su nombre de usuario.
El cliente debe haber seleccionado un menú que desee pedir.

---

### Flujo Principal
1. El cliente, en la pantalla del menú seleccionado, presiona el botón de "pedir menú".

---

### Flujos Alternativos
- **El plato ha dejado de estar disponible entre el momento en el que el usuario lo seleccionó e intentó realizar el pedido** 
  Un pop-up le informará de que el menú no está disponible y lo enviará al inicio de la aplicacion.
- **El cliente ya tiene tres pedidos activos**
  Un pop-up le avisará de que está excediendo el límite de tres pedidos y el cliente no podrá realizar el nuevo.

---

### Postcondiciones
El cliente será llevado a una pantalla donde deberá realizar el pago para confirmar el pedido.

---

### Requisitos No Funcionales
- Límite de pedidos.

---

### Prioridad
Normal.
