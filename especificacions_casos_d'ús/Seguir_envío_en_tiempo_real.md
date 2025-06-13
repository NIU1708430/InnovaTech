# Caso de Uso: Seguir Envío en Tiempo Real

### Versión
1.2

### Fecha
29/04/2025

### Autores
Elías Pascual

---

### Descripción
Aquest cas d’ús descriu com els clients poden fer un seguiment del seu enviament mitjançant la pàgina web. 
El sistema mostra la ubicació actual del repartidor en un mapa (Google Maps) amb actualització en temps real.

---

### Actores
- Cliente  
- Repartidor  
- Sistema de Mapas (Google Maps)

---

### Precondiciones
El client ha iniciat sessió i ha realitzat una comanda confirmada.
El repartidor ha iniciat el lliurament.

---

### Flujo Principal
1. El client accedeix a l’apartat de seguiment d’enviament.
2. El sistema sol·licita la ubicació actual del repartidor.
3. El sistema mostra la ubicació del repartidor en un mapa amb Google Maps.
La informació es refresca automàticament en temps real fins que el lliurament es completa.

---

### Subflujos
- El sistema pot mostrar l’estat del lliurament (en camí, prop d’arribar, lliurat).
- El client pot veure l’hora estimada d’arribada i informació de contacte del repartidor si cal.

---

### Flujos Alternativos
**Nom del flux:** Error en la localització  
- Si no es pot obtenir la ubicació del repartidor, el sistema mostra un missatge indicant la impossibilitat de mostrar el mapa.
- El sistema reintenta la connexió automàticament després d’uns segons o ofereix l’opció de reintentar manualment.

---

### Postcondición
- El sistema deixa de mostrar el seguiment un cop el lliurament s’ha completat.
- L’estat de la comanda es marca com a “lliurat”.

---

### Requisitos no funcionales
- RNF-3-01: Integració amb Google Maps.
- RNF-7-07: Ús del protocol OpenVPN per a la transmissió segura de dades.
- RNF-7-06: Temps de resposta màxim de 5 mil·lisegons un cop realitzada la petició.
- RNF-7-01: Interfície en català, castellà i anglès.

---

### Prioridad
Alta

---

### Comentarios
Aquest cas d’ús millora l’experiència del client proporcionant transparència i confiança durant el procés de lliurament.



