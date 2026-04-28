# Actividad 3: Sistema de Control de una Alarma Inteligente (Estados y Casos de Uso)

## Contexto
Un sistema de alarma para el hogar que tiene un comportamiento dinámico complejo.

---

## Parte A (Estados)

El objeto **"Sistema de Alarma"** puede estar en los siguientes estados:
- Desarmado
- Armado
- En Espera (retardo de entrada)
- Alarma Sonando
- Mantenimiento

### Comportamiento del sistema

- Si el sistema está **Armado** y se detecta movimiento:
  - Pasa a **En Espera** durante 30 segundos.

- Si en ese tiempo **no se introduce el código**:
  - Pasa a **Alarma Sonando**.

- Si se introduce el **código correcto**:
  - Pasa a **Desarmado**.

- Desde **cualquier estado**, si el técnico introduce una llave especial:
  - Pasa a **Mantenimiento**.

### Tarea
Crea el diagrama de estados detallando:
- Los **eventos**
- Las **acciones**

Ejemplo:
- Al entrar en **Alarma Sonando** → acción: `llamar_policia()`

---

## Parte B (Casos de Uso)

### Actores
- Propietario
- Sensor de Movimiento
- Central de Policía
- Técnico

### Casos de uso principales
- Armar sistema
- Desarmar sistema
- Configurar sensores
- Recibir alerta de intrusión