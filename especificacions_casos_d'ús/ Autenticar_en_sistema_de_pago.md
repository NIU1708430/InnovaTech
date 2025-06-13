# Caso de Uso: Autenticar en Sistema de Pago

### Versión
1.2

### Fecha
5/04/2025

### Autores
Elías Pascual Paz

---

### Descripción
Este caso de uso describe cómo el sistema se conecta con las plataformas de pago externas para autenticar los datos introducidos por el cliente y confirmar la transacción. 
---

### Actores
- Cliente  
- Entidad bancaria

---

### Precondiciones
- El pedido ha sido validado y está listo para procesar el pago.
- El cliente introduce los datos requeridos (por ejemplo, tarjeta o cuenta PayPal)

---

### Flujo Principal
1. El sistema establece conexión con la plataforma de pago correspondiente.
2. El sistema envía las credenciales del cliente para su validación.
3. La plataforma devuelve la respuesta de autenticación.
4. El sistema confirma si la transacción es válida.
5. El sistema registra el pago como realizado correctamente.
6. El sistema continúa con el procesamiento del pedido.

---

### Subflujos
- Si el método de pago elegido no dispone de saldo suficiente, se informa al cliente y se solicita otro método.
- Si el sistema no puede establecer conexión con la plataforma de pago, se notifica al cliente para que reintente la operación más tarde.

---

### Flujos Alternativos
**Nombre de flujo:** Error de autenticación  
- Si los datos introducidos son incorrectos, el sistema muestra un mensaje de error.
- El cliente puede reintroducir los datos o cancelar la operación.
- Si cancela, el caso de uso finaliza y el pago no se realiza.

---

### Postcondición
- El sistema ha registrado el resultado de la transacción (éxito o fallo).
- Si es exitoso, el pedido sigue su curso. Si falla, queda pendiente de pago.

---

### Requisitos no funcionales
- RNF-4-01: Integración con plataformas de pago externas (PayPal y tarjetas bancarias).
- RNF-4-02: Seguridad en transacciones cifradas.
- RNF-7-07: Uso de protocolo OpenVPN para encriptación de datos.

---

### Prioridad
Alta

---

### Comentarios
Este caso de uso es crítico para el flujo de pedidos en QueMenges, ya que garantiza que los pagos se autentiquen correctamente antes de continuar con el envío del pedido.





