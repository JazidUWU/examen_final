# Fase 2 - Desarrollo Simulado

## 1. Descomposición de Historias (Tareas Técnicas)

### H.U. 1 - Disponibilidad de médicos (5 SP)
*   **UX/UI:** Diseñar vista de calendario y selección de fechas disponibles.
*   **Frontend:** Consumir endpoint de horarios y renderizar el calendario interactivo.
*   **Backend:** Crear endpoint `GET /api/medicos/{id}/disponibilidad` consultando la base de datos de turnos.
*   **QA:** Pruebas unitarias de la respuesta del endpoint y validación de fechas pasadas en frontend.

### H.U. 2 - Reserva de citas (8 SP)
*   **UX/UI:** Diseñar formulario de confirmación de reserva y mensaje de éxito.
*   **Frontend:** Integrar formulario con endpoint POST y manejar errores de concurrencia.
*   **Backend:** Crear endpoint `POST /api/citas/reservar` con bloqueo transaccional (para evitar overbooking).
*   **QA:** Pruebas de estrés para reservas simultáneas y validación de inserción en base de datos.

### H.U. 7 - Validación de aseguradora (5 SP)
*   **UX/UI:** Diseñar campo para ingresar número de póliza y mostrar estado (Activo/Inactivo).
*   **Frontend:** Conectar input de póliza con API de aseguradoras.
*   **Backend:** Crear integración (o Mock) con API externa de Seguros para validar cobertura `GET /api/seguros/validar/{poliza}`.
*   **QA:** Pruebas con números de póliza inválidos y caídas de servicio de la API externa.

---

## 2. Identificación de Impedimentos
Para el Daily Scrum, hemos detectado estos posibles impedimentos:
1.  **Impedimento Técnico:** Si la API externa de la aseguradora (para H.U. 7) se cae o no responde, el flujo de reserva se bloquea.
2.  **Impedimento Operativo:** Asegurarnos de que el esquema de la base de datos para los horarios (H.U. 1) soporte múltiples zonas horarias si el centro médico tiene varias sucursales.
