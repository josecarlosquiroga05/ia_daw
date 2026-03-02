# ia_daw
# Práctica IA (RA4 · b+c) — Big Data, análisis, rentabilidad y valoración IA

## 1) Caso y objetivo de negocio
Empresa/sector (real o ficticia): Netflix (sector streaming audiovisual)

Problema a resolver: Alta rotación de usuarios (churn) y dificultad para maximizar el tiempo de visualización.

Objetivo de negocio (rentabilidad): Aumentar retención y tiempo de consumo para incrementar ingresos recurrentes y reducir cancelaciones.

## 2) Big Data: recogida masiva de datos
Es Big Data porque combina gran volumen, alta velocidad de generación y gran variedad de formatos.

Fuente 1: Historial de visualización (qué se ve, cuándo, cuánto tiempo).

Fuente 2: Interacciones del usuario (pausas, rebobinado, búsquedas, valoraciones).

Fuente 3: Datos contextuales (dispositivo, ubicación aproximada, franja horaria).

Volumen/velocidad (estimación):
Millones de usuarios activos diarios generando miles de millones de eventos de reproducción al día en tiempo real.

Formatos:
Eventos (logs), texto (búsquedas), metadatos audiovisuales, series temporales de consumo.

## 3) Tratamiento/análisis: pipeline de datos
Ingesta (captura/eventos):
Captura automática de eventos cada vez que el usuario interactúa con la plataforma.

Limpieza/normalización:
Eliminación de datos duplicados, anonimización y estandarización de formatos.

Almacenamiento (data lake/warehouse):
Data lake distribuido en la nube y posterior estructuración en data warehouse para análisis.

Preparación de variables (features):
Variables como: género preferido, frecuencia de uso semanal, tasa de abandono de series, horario habitual.

Análisis/BI (opcional):
Paneles internos para analizar tendencias de consumo por país, edad o contenido.

## 4) IA aplicada: modelo y decisión
Tipo de IA/técnica:
Sistemas de recomendación (machine learning predictivo + filtrado colaborativo).

Entrada del modelo:
Historial de consumo, similitud con otros usuarios, metadatos de contenido.

Salida del modelo:
Ranking personalizado de contenidos con probabilidad estimada de visualización.

Decisión que habilita:
Mostrar recomendaciones personalizadas en la portada para maximizar tiempo de visualización y reducir cancelación.

## 5) Rentabilidad: KPIs antes/después (mínimo 3)
KPI 1 (Tasa de retención mensual):

Antes: 85%

Después: 90%

Por qué mejora la rentabilidad:
Más retención implica más ingresos recurrentes sin coste adicional de adquisición.

KPI 2 (Tiempo medio de visualización diario):

Antes: 70 minutos

Después: 95 minutos

Por qué mejora la rentabilidad:
Mayor engagement reduce probabilidad de cancelación y aumenta valor de vida del cliente (LTV).

KPI 3 (Tasa de cancelación mensual – churn):

Antes: 5%

Después: 3%

Por qué mejora la rentabilidad:
Menor churn reduce costes de marketing necesarios para captar nuevos usuarios.

## 6) Diagrama del pipeline (ASCII o Mermaid)
 Usuarios
        │
        ▼
Captura de eventos (logs)
        │
        ▼
  Limpieza / Normalización
        │
        ▼
    Data Lake (almacenamiento masivo)
        │
        ▼
Feature Engineering (variables)
        │
        ▼
  Modelo IA Recomendador
        │
        ▼

Recomendaciones personalizadas
        │
        ▼
↑ Mayor retención y rentabilidad ↑

## 7) Riesgos y mitigación
Riesgo 1: Sesgo algorítmico (mostrar siempre contenidos similares).

Mitigación 1: Introducir diversidad controlada y exploración en el algoritmo.

Riesgo 2: Problemas de privacidad de datos.

Mitigación 2: Anonimización, cifrado y cumplimiento de normativas como Reglamento General de Protección de Datos (RGPD).

## 8) Valoración (criterio c): importancia presente y futura de la IA (10–15 líneas)
Importancia actual (hoy):
La IA es un elemento estructural en empresas digitales. Permite personalización masiva, optimización de costes y toma de decisiones basada en datos en tiempo real. Sin IA, plataformas como Netflix perderían competitividad frente a otros actores del sector.

Importancia futura (3–5 años):
La IA evolucionará hacia modelos generativos, automatización de producción audiovisual, predicción avanzada de tendencias y creación de contenido personalizado dinámicamente.

Condiciones/limitaciones:
Requiere grandes volúmenes de datos, inversión tecnológica elevada, regulación estricta en privacidad, y gestión ética del impacto laboral.

Conclusión razonada:
La IA no solo mejora procesos, sino que redefine modelos de negocio basados en suscripción. En el futuro, será un factor determinante de liderazgo empresarial y diferenciación competitiva.

## 9) Fuentes oficiales (mín. 2)
- Big Data/analítica (enlace oficial): https://netflixtechblog.com/
- IA/técnica/modelo (enlace oficial): https://research.netflix.com/
