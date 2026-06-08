# Estimación, Dependencias y Selección (Sprint Backlog)

## 1. Estimación de Historias (Fibonacci)
Considerando la complejidad técnica (Frontend, Backend, QA y UX), esta es una propuesta de estimación para cada historia:

1. **Disponibilidad de Médicos:** 5 SP *(Complejidad media: requiere lógica de calendarios y horarios).*
2. **Validación Aseguradora:** 5 SP *(Complejidad media: validación de datos o posible mock de API).*
3. **Reserva de Citas:** 8 SP *(Complejidad alta: lógica transaccional, bloqueos de horarios y confirmación).*
4. **Notificaciones:** 3 SP *(Complejidad baja: envío de correos de confirmación).*
5. **Historial Médico:** 8 SP *(Complejidad alta: seguridad de datos sensibles y CRUD).*
6. **Resultados de Laboratorio:** 8 SP *(Complejidad alta: integración para subida y lectura de documentos).*
7. **Pagos Online:** 13 SP *(Complejidad muy alta: integración con pasarela de pagos).*

**Suma Total del Backlog:** 50 SP (Excede nuestra capacidad de 34 SP, por lo que debemos descartar algunas para este Sprint).

---

## 2. Identificación de Dependencias
* **Reserva de Citas** *depende de* **Disponibilidad de Médicos** (No puedes reservar si no sabes qué horarios hay libres).
* **Reserva de Citas** *depende de* **Validación Aseguradora** (Según el Sprint Goal, debe validarse el seguro durante el proceso de reserva).

---

## 3. Selección de Historias (Sprint Backlog)
Para cumplir con el **Sprint Goal** de entregar el MVP exitoso, seleccionamos obligatoriamente las siguientes historias y aprovechamos el espacio sobrante para añadir valor rápido (Notificaciones):

| Historia Seleccionada | Puntos (SP) |
| :--- | :---: |
| 1. Disponibilidad de Médicos | 5 SP |
| 2. Validación Aseguradora | 5 SP |
| 3. Reserva de Citas | 8 SP |
| 4. Notificaciones (Valor Agregado) | 3 SP |
| **Total Comprometido** | **21 SP** |

*(21 SP está dentro de nuestra capacidad máxima de 34 SP, dejando un margen seguro para imprevistos).*

### Historias descartadas para próximos Sprints:
* Historial Médico (8 SP)
* Resultados de Laboratorio (8 SP)
* Pagos Online (13 SP)
