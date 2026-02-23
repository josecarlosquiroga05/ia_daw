# ia_daw

# Práctica IA (RA4 · a) — Automatización y optimización

## 1) Proceso elegido
- Nombre del proceso: Clasificación de tickets de soporte
- Contexto (empresa/servicio web/IT): Empresa de servicios TI que ofrece soporte a clientes mediante un sistema de tickets.
- Rol/es implicados: Soporte técnico, agentes de atención al cliente, equipo de IT.

## 2) ANTES (sin IA)
- Pasos (5–7):
  1. El cliente presenta una solicitud de soporte a través de un formulario en línea.
  2. El sistema genera un ticket de soporte y lo envía al equipo de atención.
  3. Un agente humano recibe el ticket y lo clasifica manualmente según el tipo de problema (por ejemplo, errores en el sistema, problemas de acceso, consultas generales).
  4. El agente asigna el ticket al equipo o nivel de soporte adecuado según la clasificación.
  5. El equipo de soporte resuelve el ticket o, en algunos casos, lo escalan a un nivel superior.
- Tiempo aproximado por caso: 10-15 minutos por ticket.
- Problemas / cuellos de botella:
  - Errores humanos en la clasificación.
  - Falta de priorización adecuada de los tickets.
  - Alta carga de trabajo que genera retrasos y agotamiento.
  - Variabilidad en la clasificación de tickets entre agentes.

## 3) DESPUÉS (con IA)
- ¿Qué automatiza la IA?
  - Clasificación automática de tickets.
  - Priorización automática de los tickets según su urgencia.
- ¿Qué queda para humanos?
  - Resolución de tickets complejos.
  - Validación de tickets cuando la IA no tiene suficiente confianza.
  - Gestión de excepciones y escalado de problemas.
- Datos necesarios (tipos de datos, sin datos personales):
  - Texto: Descripciones de los tickets.
  - Historial de tickets: Clasificación previa, etiquetas, resultados.
  - Metadatos: Fecha, prioridad, asignación, etiquetas.
- Modelo/técnica (NLP, clasificación, recomendación, visión, etc.):
  - Procesamiento de lenguaje natural (NLP).
  - Modelos de clasificación supervisada.
  - Análisis de sentimiento.

## 4) Optimización (mejora medible)
Define 3 métricas con valores antes/después:
- Tiempo:
  - Antes: 10-15 minutos por ticket.
  - Después: 2-3 minutos por ticket.
- Coste:
  - Antes: 8 horas/día por agente en clasificación.
  - Después: 25-30% de reducción de costes operativos.
- Calidad:
  - Antes: Tasa de clasificación errónea del 15-20%.
  - Después: Tasa de clasificación errónea reducida a 5-10%.

## 5) Diagrama del flujo (ASCII o Mermaid)
```mermaid
flowchart LR
  A[Cliente crea ticket] --> B[IA clasifica ticket]
  B --> C[IA asigna prioridad]
  C --> D[IA asigna equipo]
  D --> E[Agente humano valida (si necesario)]
  E --> F[Resolución o escalado]
  F --> G[Ticket cerrado]

## 6) Riesgos y mitigación
Riesgo 1: Sesgo en la clasificación. La IA puede replicar sesgos de los datos históricos.
Mitigación 1: Auditoría periódica de resultados y entrenamiento con datos balanceados.

Riesgo 2: Dependencia de la IA y falta de trazabilidad. Los agentes podrían confiar demasiado en la IA.
Mitigación 2: Mantener un humano en el bucle para validación y asegurar trazabilidad completa de la clasificación.

7) Fuente oficial

Enlace: https://scikit-learn.org/stable/modules/feature_extraction.html#text-feature-extraction
