# README de la Actividad 1

## Actividad 1: Sistema de Gestión de un Centro Deportivo (Casos de Uso y Actividades)

### Contexto
Un centro deportivo quiere digitalizar su reserva de pistas de pádel y clases dirigidas.

---

## Parte A (Casos de Uso)

- Los **Socios** pueden:
  - Identificarse
  - Reservar una pista
  - Apuntarse a clases

- Para **reservar una pista**, el sistema siempre debe verificar si el socio tiene pagos pendientes (**include**).

- Al **apuntarse a una clase**, el socio puede, si quiere, contratar un seguro de lesiones opcional (**extend**).

- El **Administrador** puede:
  - Dar de alta nuevas clases
  - Gestionar los pagos de los socios

### Tarea
Dibuja el diagrama de casos de uso incluyendo:
- Actores
- Relaciones de inclusión
- Relaciones de extensión
- Herencia (si fuera necesario)

---

## Parte B (Actividades)

Dibuja el diagrama de actividades del proceso **"Reservar una pista"**.

### Flujo del proceso

1. El proceso comienza con el socio eligiendo **fecha y hora**.
2. El sistema comprueba la **disponibilidad**.
3. Si **no hay pista disponible**:
   - El socio puede elegir otra fecha **o salir**.
4. Si **hay pista disponible**:
   - Se comprueba si tiene **pagos pendientes**.
   - Si **debe dinero** → se deniega la reserva.
   - Si **está al día**:
     - Se confirma la reserva.
     - Se envía un **email de confirmación**.