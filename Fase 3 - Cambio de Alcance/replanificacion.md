# Fase 3 - Cambio de Alcance (Replanificación)

## 1. Nuevas Restricciones del Negocio
Durante el desarrollo del Sprint, se han introducido las siguientes restricciones sorpresivas:

![Fotografía de Restricciones](../Fase%201%20-%20Sprint%20Planning/Entregables%20Fotograficos/foto_restricciones.jpg)

1.  **Solo existe presupuesto para el MVP.**
2.  **La API de laboratorio es inestable.**
3.  **El negocio necesita demostrar valor rápidamente.**

## 2. Análisis de Impacto
*   **Impacto en el Presupuesto y Valor rápido:** Nos confirma que nuestra decisión en la Fase 1 de enfocarnos únicamente en 3 historias (18 SP) descartando Pagos y Notificaciones fue **100% correcta**. No hay margen para lujos.
*   **Impacto de la API inestable:** Esto afecta directamente y de manera crítica a nuestra **H.U. 7 - Validación de aseguradora (laboratorio)**. Si la API se cae, no podemos terminar la historia y el Sprint fracasaría.

## 3. Ajuste de Alcance (Solución Propuesta)
Para adaptarnos al cambio sin fallar el Sprint, el equipo de desarrollo debe tomar una acción inmediata sobre el Sprint Backlog:

**Decisión Ágil:**
*   **Ajustar la H.U. 7:** En lugar de conectarnos a la API real del laboratorio (que es inestable), el equipo de Backend desarrollará un **Mock** (simulador) de la API o se implementará una validación "manual" temporal. 
*   **Justificación:** Esto nos permite "demostrar valor rápidamente" (como pide el negocio), habilitar el flujo de reservas para el MVP y no quedarnos bloqueados por un proveedor externo inestable.

El Sprint Backlog se mantiene en **H.U. 1, H.U. 2 y H.U. 7 (Mockeada)** por 18 SP, asegurando el cumplimiento del Sprint Goal original bajo las nuevas restricciones de presupuesto.
