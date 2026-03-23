# Práctica IA (RA4 · f)

## 1) Caso de uso
- Tipo de aplicación:
  Plataforma web de e-commerce con recomendaciones inteligentes.

- Problema:
  Los usuarios no encuentran fácilmente productos relevantes, lo que reduce las ventas.

- Usuario:
  Clientes de la tienda online y administradores del negocio.


## 2) Datos
- Datos:
  Historial de compras, clics en productos, búsquedas, tiempo de permanencia, valoraciones.

- Tipo minería:
  Recomendación basada en:
  - Clasificación
  - Clustering (segmentación de usuarios)
  - Predicción (productos que probablemente comprará)


## 3) Pipeline
- Recogida:
  Logs de navegación, base de datos de usuarios, eventos de clics.

- Limpieza:
  Eliminación de datos duplicados, tratamiento de valores nulos, filtrado de ruido.

- Transformación:
  Conversión a variables numéricas, creación de perfiles de usuario, normalización.

- Entrenamiento:
  Modelo de recomendación (por ejemplo, filtrado colaborativo o machine learning supervisado).

- Predicción:
  Generación de listas de productos recomendados para cada usuario.

- Uso:
  Mostrar recomendaciones personalizadas en la app web.

  ## 4) Integración
- Backend:
  API REST que conecta la base de datos con el modelo de IA (microservicio en Python o Node.js).

- Frontend:
  Interfaz web que muestra productos recomendados en tiempo real.

- Flujo:
  Usuario entra → navega → backend recoge datos → IA procesa → devuelve recomendaciones → frontend las muestra.


## 5) Valor
- Mejora:
  Personalización de la experiencia de usuario y aumento de conversión.

- Sin IA:
  Recomendaciones genéricas poco efectivas.

- Rentabilidad:
  Incremento de ventas, fidelización del cliente y mayor tiempo en la plataforma.
  
## 6) Diagrama

Usuario 
   ↓
App Web (Frontend)
   ↓
Backend (API REST)
   ↓
Modelo de IA
   ↓
Resultado (Recomendaciones)
   ↓
Usuario

