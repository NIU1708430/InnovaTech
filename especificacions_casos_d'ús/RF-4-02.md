# Caso de Uso: Autenticar en Sistema de Pago

### Versión
1.1

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
1. La plataforma verifica la validez de los datos y confirma la autenticación.
2. El sistema recibe la confirmación de la transacción.
3. El sistema registra el pago como exitoso y continúa con el procesamiento del pedido.

---





