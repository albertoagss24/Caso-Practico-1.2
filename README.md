# Repo para Caso Práctico 1.2 - DevOps&Cloud UNIR

El Caso Práctico 1.2 consiste en ampliar el pipeline del CP1.1 (que ya tenemos funcionando con etapas Get Code, Build, Unit y Rest) para incluir nuevas pruebas de calidad, distribuirlo en 3 agentes Jenkins y subir la cobertura del código al 100%.

Las tareas o retos a trabajar en este apartado son:

- Replicar todo el ejemplo del pipeline visto en clase, en el PC de cada alumno, y preparar los mismos entregables que en el primer reto:
    • URL al repositorio del alumno con el código fuente y el Jenkinsfile.
       Este código fuente debe estar en la rama “master”.
    • Log de la ejecución del pipeline.
    • Captura de pantalla de la ejecución del pipeline y las gráficas de evolución de los test unitarios/integración, seguridad, estático, cobertura y rendimiento.
    • Explicación del funcionamiento del pipeline.

Puntuación: 60 %.

- Separar la ejecución del pipeline en 3 agentes (principal, y dos secundarios) a libre elección del alumno y con toda la concurrencia que sea posible. Esos agentes, al no compartir el workspace, deberán usar los mecanismos de intercambio de archivos de Jenkins y de limpieza del repositorio.
    • URL al repositorio del alumno con el código fuente y el nuevo Jenkinsfile (diferente al que debe contener el apartado anterior).
    • El código fuente no cambia y debe permanecer en master, pero se actualizará el Jenkinsfile que ya se trabajó en el apartado anterior para este mismo propósito (p.e. “<raiz>\JENKINSFILE_agentes”).
    • Log de la ejecución del pipeline (debe visualizarse un “whoami” y “hostname” para identificar el agente empleado en cada etapa).
    • Log y explicación sobre lo que ocurre cuando el número de “executors” (o unidades de ejecución de nuestros agentes) lo reducimos a 1, teniendo 4 etapas ejecutándose simultáneamente en 2-3 agentes.
    • Explicación de la separación de agentes que se ha decidido realizar.

Puntuación: 25 %.

- Mejora de las pruebas de cobertura (por líneas y por caminos “branches”) para lograr una cobertura total del código (100 %). Solo debe modificarse el código fuente de la carpeta “test”; en ningún caso se tocará el código fuente de la carpeta “app” para este ejercicio.
    • URL al repositorio del alumno con el nuevo código fuente.
       Debe entregarse en rama “feature_fix_coverage”.
    • Log de la ejecución del pipeline en rama master donde no se consigue una cobertura completa, y mismo log sobre la rama “feature_fix_coverage” donde sí se consigue la cobertura completa.
    • Explicación de cómo se ha realizado la mejora y por qué antes no se alcanzaba el 100% de cobertura.

Puntuación: 15%.
