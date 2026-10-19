# SJA-UTA — APE 3

Proyecto de Estructura de Datos de Ingeniería de Software de la Universidad Técnica de Ambato.

El Sistema Jerárquico Académico UTA utiliza dos estructuras:

- Un árbol general para representar la organización académica: universidad, facultades, carreras, niveles y paralelos.
- Un árbol binario de búsqueda por cada paralelo para gestionar estudiantes ordenados por matrícula.

## Organización del repositorio

| Carpeta                    | Contenido                                                                                                                                                         |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Grupo1](Grupo1/README.md) | Fase 1: caso práctico, modelos, enumerados, diagramas, datos de prueba y código base.                                                                             |
| [Grupo2](Grupo2/README.md) | Fase 2: inserción, búsqueda, recorridos recursivos, trazas y consultas del árbol general. Incluye modificación y eliminación del ABB como adelantos de la Fase 3. |

## Fase 1 — Modelado y estructura base

El Grupo 1 define el caso SJA-UTA, las clases, las relaciones, las reglas jerárquicas y los datos de prueba.

La organización utiliza un árbol general porque una unidad puede tener varios hijos. Cada paralelo contiene su propio ABB de estudiantes.

- [Documentación del Grupo 1](Grupo1/README.md)

## Fase 2 — Implementación recursiva

El Grupo 2 continúa sobre la estructura base e incorpora:

- Agregar y buscar unidades académicas.
- Mostrar la jerarquía con sangría.
- Consultar grado y nivel.
- Contar hojas.
- Insertar estudiantes sin matrículas repetidas.
- Buscar estudiantes por matrícula.
- Obtener preorden, inorden y posorden.
- Mostrar trazas de las llamadas recursivas.
- Modificar y eliminar estudiantes como adelantos de la Fase 3.

La altura del árbol general sigue pendiente en la copia revisada. Su resultado esperado con los datos iniciales es de cuatro aristas.

### Documentación

- [README del Grupo 2](Grupo2/README.md)
- [Casos de prueba](Grupo2/docs/casos_prueba.md)
- [Decisiones de implementación](Grupo2/docs/decisiones.md)
- [Diagramas de flujo](Grupo2/docs/diagramas-flujo/README.md)
- [Diagramas de secuencia](Grupo2/docs/diagramas-secuencia/README.md)
- [Trazas de recorridos](Grupo2/docs/trazas_recorridos.md)
- [Trazas de inserción y eliminación](Grupo2/docs/trazas_insercion_eliminacion.md)

### Facilitación de la clase

La Fase 2 utiliza cuatro estaciones: inserción, preorden, inorden y posorden, y caza del error recursivo.

Los grupos publican sus respuestas en el Padlet de la actividad.

- [Organización de las estaciones](Grupo2/facilitacion/estaciones/README.md)
- [Lista de cotejo](Grupo2/facilitacion/lista-cotejo-fase2.md)
- [Enlaces y recursos](Grupo2/facilitacion/enlaces.md)

## Continuación para la Fase 3

Las operaciones pendientes previstas para la siguiente fase son:

- Eliminar unidades del árbol general.
- Transformar el árbol general a una representación binaria.
- Calcular altura y estadísticas del ABB: cantidad de estudiantes, menor matrícula, mayor matrícula y promedio general.

La modificación y la eliminación de estudiantes ya están implementadas por el Grupo 2.

## Ejecución

Consultar las instrucciones del README de cada grupo.

Los proyectos se compilan por separado porque contienen clases con los mismos nombres y paquetes. No compilar juntos los archivos Java de Grupo1 y Grupo2.

La guía solicita JDK 21. El código del Grupo 2 también se comprobó con Java 17.

## Trabajo colaborativo

Cada integrante trabaja en su rama y abre un pull request hacia main.

Damián revisa e integra los aportes del Grupo 2. Después de integrar, se comprueban los resultados y se actualiza la documentación.
