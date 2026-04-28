# Actividad 2: Máquina Expendedora de Billetes de Metro (Actividades y Estados)

## Contexto
Vamos a modelar la lógica de una máquina automática donde el comportamiento depende mucho del estado del objeto **"Billete"** y de la lógica del proceso.

---

## Parte A (Actividades)

Representa el flujo de **"Comprar Billete"**:

1. El usuario selecciona el destino.
2. El sistema calcula el precio.
3. El usuario introduce:
   - **Monedas (efectivo)**, o
   - **Tarjeta**

### Condiciones:
- Si es **tarjeta**:
  - Conectar con el banco
  - Validar el PIN

- Si es **efectivo**:
  - Comprobar si la máquina tiene cambio

### Resultado final:
- Una vez pagado:
  - Se imprime el billete
  - Se entrega el cambio (si corresponde)

---

## Parte B (Estados)

Dibuja el diagrama de estados del objeto **"Billete"**.

### Estados sugeridos:
- No emitido
- Emitido / Activo
- Validado (en uso)
- Agotado
- Caducado

### Tarea
Indica qué **eventos provocan el cambio de estado**.

Ejemplo:
- El evento **"picar en el torno"** provoca el cambio de **Emitido** a **Validado**.