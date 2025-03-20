# Módulo 8 - Ejercicio pŕactico 1

## Preguntas teóricas:

1.  Fundamentos de DevOps (0.5 pts)

    - ¿Qué es DevOps y cuál es su propósito principal?

      Es una filosofía de trabajo que combina las prácticas y herramientas de los equipos de desarrollo y operaciones, mejorando la colaborarión entre ambos equipos para acelerar la entrega de software y asegurar que este cumple ciertos requisitos de calidad.

      Los principios fundamentales de DevOps son Colaboración continua, Automatización, Retroalimentación continua y Mejora continua.

    - Explica el modelo CAMS y su importancia en la cultura DevOps.

      El modelo CAMS establece los cuatro pilares esenciales de DevOps:

      1.  **Culture (Cultura):** Fomenta la colaboración entre equipos, eliminando los silos.
      2.  **Automation (Automatización):** Automatiza tareas manuales repetitivas, como las pruebas y el despliegue.
      3.  **Measurement (Medición):** Monitorea y mide continuamente el rendimiento del sistema y los equipos.
      4.  **Sharing (Compartir):** Fomenta la transparencia y el intercambio de conocimiento entre los miembros del equipo.

      Gracias a este modelo, se cumplen los principios fundamentales mencionados en la pregunta anterior.

2.  Integración y Entrega Continua (0.5 pts)

    - ¿Cuál es la diferencia entre Integración Continua y Entrega Continua?

      - **Integración Continua (CI)**: Los cambios de código se integran automáticamente en un repositorio central en el cual se ejecutan pruebas automatizadas de integración.

      - **Entrega Continua (CD)**: Es el despliegue automático de código en entornos de prueba y producción.

    - ¿Qué beneficios aporta la Integración Continua al proceso de desarrollo de software?
      - Las pruebas de integración continua permiten la detección temprana de errores.
      - Esta detección temprana de erroes reduce el riesgo de errores más costosos en una etapa futura.
      - Aceleración en el ciclo de desarrollo gracias a la automatización de tareas repetitivas

3.  Contenedores y Docker (0.5 pts)

    - ¿Qué es un contenedor y en qué se diferencia de una máquina virtual?

      Un contenedor es un entorno aislado en el cual se ejecuta un proyecto o aplicación. Utiliza el núcleo del sistema operativo anfitrión, pero este entorno aislado contiene solo los binarios especificados en su archivo de configuración.

      **A diferencia de una máquina virtual, no virtualiza un sistema operativo completo**, solo ejecuta los binarios y librerias necesarias de la aplicación, lo que lo hace más liviano y su ejecución es más rápida.

    - ¿Cuáles son los beneficios del uso de Docker en entornos DevOps?

      El principal beneficio es **que el entorno de desarrollo es similar al entorno de producción**, evitando errores producidos por diferencias en entornos de ejecución.

4.  Pruebas y Automatización en CI/CD (0.5 pts)

    - ¿Cuáles son los tipos de pruebas más importantes en un pipeline de CI/CD?

      Las pruebas que están relacionadas con entregar una aplicación estable son:

      - Pruebas unitarias: Certifican que las funcionalidades que se estan implementando funcionan adecuadamente en distintos casos de uso, evitando errores que podrían suceder en casos "no cosiderados por el programador".
      - Pruebas de integración: Valida que la nueva funcionalidad funcione bien con el resto de la aplicación.
      - Pruebas de aceptación: valida que la aplicación cumpla todos los criterios de aceptación establecidos.

      Tambien existen otros tipos de pruebas, que no son menos importantes, pero atienden otras necesidades adicionales a los requerimientos.

      - Pruebas de rendimiento: Se prueba la aplicación con diferentes cargas de trabjo.
      - Pruebas de seguridad: Se buscan las diferentes vulnerabilidades de la aplicación.

    - Explica en qué consiste el desarrollo guiado por pruebas (TDD) y su impacto en CI/CD.

      El desarrollo guiado por pruebas, consiste en que el desarrollador se basa en que la funcionalidad que se está desarrollando tiene como objetivo pasar cierta prueba (que inicialmente no pasa). Una vez que pasa esta prueba, el desarrollador puede refinar el código tratando de siga pasando exitósamente la prueba.

5.  Infraestructura y Monitoreo en DevOps (0.5 pts)

    - ¿Qué es Infraestructura como Código (IaC) y qué ventajas ofrece?

      La IaC consite gestionar la infraestructura de ejeccución mediante código en vez de reqalizar configuraciones manuales. Esto permite la automatización de la creación, gestion y mantenimiento de las infraestructuras.

    - ¿Por qué es importante el monitoreo en DevOps? Menciona al menos dos herramientas de monitoreo utilizadas en entornos CI/CD.

      El monitoreo entrega informacion inmediata sobre el estado del sisterma después de cada despliegue, evitando la introducción de errores o fallas en rendimiento del sistema.

6.  Orquestación y Kubernetes (0.5 pts)

    - ¿Cuál es el propósito de un orquestador de contenedores como Kubernetes?

      Los orquestadores de contenedores controlan el despliegue de múltiples contenedores de aplicación. Se usan para manejar grandes cantidades de contenedores en producción, asegurando que se escalen y distribuyan de forma automática.

    - Explica cómo Kubernetes facilita la escalabilidad y gestión de aplicaciones en producción.

      Kubernetes ofrece diversas ventajas en torno a escalibiladad y gestion de aplicaciones.

      - Tiene un sistema de despliegue declarativo, por lo que se le puede indicar en que estado se quiere correr una aplicacion y kubernetes gestionará los recursos para llegar a ese estado.
      - Puede gestionar réplicas de una aplicación y relizar un balanceo de carga, para optimizar el rendimiento.

## Informe

1. Introducción (0.5 pts)
   - Breve descripción del proyecto en el que se aplicarán los conceptos de DevOps.
2. Aplicación de Integración y Entrega Continua (1 pt)
   - Explicación de cómo configurarían un pipeline de CI/CD utilizando herramientas como Jenkins, GitLab CI o CircleCI.
   - Pasos para integrar pruebas automatizadas en el pipeline.
3. Uso de Contenedores y Orquestación (1 pt)
   - Cómo implementarían Docker en el proyecto.
   - Ventajas de utilizar Docker y Kubernetes en el despliegue del sistema.
4. Monitoreo y Seguridad en DevOps (1.5 pts)
   - Estrategias para monitorear logs y métricas del sistema.
   - Uso de herramientas de monitoreo como ELK Stack o Prometheus para asegurar la estabilidad del proyecto.
