# Caso de Uso: Valorar Pedido

### Versión
1.2

### Fecha
06/05/2025

### Autores
Elías Pascual Paz

---

### Descripción
Este caso de uso permite al cliente realizar una valoración de su pedido una vez ha sido entregado.

---

### Actores
- Cliente

---

### Precondiciones
- El cliente ha iniciado sesión
- El pedido se encuentra en estado “entregado”

---

### Flujo Principal
1. El cliente accede al historial de pedidos y selecciona uno finalizado.
2. El cliente indica su nivel de satisfacción en varios aspectos.
3. El sistema guarda la información y la asocia al pedido, al cocinero y al repartidor correspondientes.

---

### Subflujos
- El cliente puede añadir un comentario adicional junto con la valoración numérica.
- El cliente puede editar la valoración dentro de un límite de tiempo (por ejemplo, 24h después del pedido).

---

### Flujos Alternativos
**Nombre del flujo:** Pedido no valorable  
- Si el pedido aún no ha sido entregado, el sistema no permite su valoración y muestra un mensaje informativo.

**Nombre del flujo:** Valoración ya realizada  
- Si el pedido ya ha sido valorado, el sistema informa al cliente y ofrece la opción de visualizar su valoración (si es editable, también modificarla).

---

### Postcondición
- La valoración queda registrada en el sistema.
- Se actualiza el perfil del cocinero con la nueva puntuación recibida, lo que puede influir en su posicionamiento dentro de la aplicación.

---

### Requisitos no funcionales
- RNF-5-01: Valoración del pedido (puntualidad y estado de la comida).
- RNF-5-02: A mayor valoración, mejor posición del cocinero en el listado de platos.

---

### Prioridad
Media

---

### Comentarios
La calidad del sistema de valoraciones es clave para fomentar la confianza entre usuarios y cocineros, y para mantener una oferta competitiva y fiable en la plataforma.

