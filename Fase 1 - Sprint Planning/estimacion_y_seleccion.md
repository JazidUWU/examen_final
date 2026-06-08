# Estimación, Dependencias y Selección (Sprint Backlog)

## 1. Estimación de Historias (Fibonacci)
Manteniendo la estimación anterior para cada historia numerada:

1. **H.U. 1 - Disponibilidad de Médicos:** 5 SP
2. **H.U. 2 - Reserva de Citas:** 8 SP
3. **H.U. 3 - Historial Médico:** 8 SP
4. **H.U. 4 - Notificaciones:** 3 SP
5. **H.U. 5 - Resultados de Laboratorio:** 8 SP
6. **H.U. 6 - Pagos Online:** 13 SP
7. **H.U. 7 - Validación Aseguradora:** 5 SP

**Suma Total del Backlog:** 50 SP (Excede la capacidad de 34 SP).

---

## 2. Identificación de Dependencias
De acuerdo a la nueva fotografía, estas son las reglas estrictas:

![Fotografía de Dependencias](foto_dependencias.jpg)

* **H.U. 2** depende de **H.U. 1** (Reserva depende de Disponibilidad).
* **H.U. 6** depende de **H.U. 2** (Pagos depende de Reserva).
* **H.U. 4** depende de **H.U. 6 y H.U. 2** (Notificaciones depende de Pagos y Reserva).
* **H.U. 5** depende de **H.U. 7** (Resultados Lab. depende de Validación Aseguradora).

---

## 3. Selección de Historias (Sprint Backlog)
Para cumplir el **Sprint Goal**, necesitamos la **H.U. 1**, **H.U. 2** y **H.U. 7**.
Si observamos las dependencias, incluir la **H.U. 4 (Notificaciones)** nos obliga a incorporar primero la **H.U. 6 (Pagos Online)**. 

Calculando la suma, podemos incluir todas estas historias usando nuestra capacidad al máximo sin sobrepasarla:

| Historia Seleccionada | Puntos (SP) |
| :--- | :---: |
| 1. H.U. 1 - Disponibilidad de Médicos | 5 SP |
| 2. H.U. 2 - Reserva de Citas | 8 SP |
| 3. H.U. 7 - Validación Aseguradora | 5 SP |
| 4. H.U. 6 - Pagos Online | 13 SP |
| 5. H.U. 4 - Notificaciones | 3 SP |
| **Total Comprometido** | **34 SP** |

¡El equipo aprovechará exactamente el 100% de su capacidad inicial (34 SP) respetando perfectamente todas las dependencias lógicas del examen!

### Historias descartadas para próximos Sprints:
* H.U. 3 - Historial Médico (8 SP)
* H.U. 5 - Resultados de Laboratorio (8 SP)
