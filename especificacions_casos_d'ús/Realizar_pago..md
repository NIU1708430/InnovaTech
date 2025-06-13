# Caso de Uso: Realizar Pago

### Versión
1.2

### Fecha
30/04/2025

### Autores
Elías Pascual Paz

---

### Descripción
Este caso de uso describe cómo el cliente selecciona un método de pago y efectúa el pago del pedido. La aplicación permite pagar mediante tarjeta bancaria o PayPal.

---

### Actores
- Cliente  
- Entidad bancaria

---

### Precondiciones
- El cliente ha iniciado sesión.
- El cliente ha finalizado la selección de platos y confirmado el pedido.
- El sistema ha calculado el total del pedido incluyendo el coste de envío.

---

### Flujo Principal
1. El cliente accede al proceso de pago tras confirmar su pedido.
2. El sistema muestra las opciones de pago disponibles.
3. El cliente introduce sus datos de pago y confirma la transacción.
4. El sistema recibe la confirmación del pago y finaliza el proceso de pedido.


---

### Subflujos
- El cliente puede modificar el método de pago antes de confirmar la transacción.
- El sistema recalcula el importe total si se aplican descuentos mediante puntos acumulados.

---

### Flujos Alternativos
**Nombre de flujo:** Pago cancelado  
- El cliente decide cancelar el pago.
- El sistema notifica la cancelación y mantiene el pedido en estado pendiente de pago.

**Nombre de flujo:** Error en el método de pago  
- Si la plataforma de pago devuelve un error (por datos inválidos o problemas técnicos), el sistema informa al cliente.
- El cliente puede reintentar o seleccionar otro método de pago.

---

### Postcondición
- El pedido queda marcado como pagado en el sistema.
- El sistema queda listo para iniciar el proceso de envío.

---

### Requisitos no funcionales
- RNF-4-01: Métodos de pago aceptados (tarjeta bancaria y PayPal).
- RNF-4-02: Conexión segura con plataformas de pago externas.
- RNF-4-03: Distribución del pago entre cocinero y repartidor tras la transacción.

---

### Prioridad
Alta

---

### Comentarios
El sistema debe garantizar una experiencia de pago fluida y segura, permitiendo que el cliente finalice su pedido con éxito y confianza.

