# Bibliografía Fundamental
**(El Arsenal de la Física Organizacional)**

### Introducción: Las Fuentes de la Arquitectura
Este anexo no es una lista de lectura académica para gerentes; es el marco teórico innegociable de la **Física Organizacional**. Hemos seleccionado las obras fundacionales de la teoría de sistemas, la cibernética, la ingeniería de confiabilidad y la termodinámica del riesgo. Estos textos proveen la base matemática y estructural para destruir el "teatro documental" y transformar la gestión de riesgos en una inecuación de latencia e infraestructura de contención.

### Bloque 1: La Termodinámica del Desastre (Acoplamiento y Complejidad)

* **Perrow, C. (1984).** "Normal Accidents: Living with High-Risk Technologies". Princeton University Press. [[Ver Libro]](https://www.amazon.com/Normal-Accidents-Living-High-Risk-Technologies/dp/0691004129)
    * **Por qué leerlo:** El texto fundacional que demuestra que el colapso no es un "error humano", sino una propiedad estructural. Establece los conceptos de "Interacciones Complejas" y "Acoplamiento Fuerte" (Tight Coupling), demostrando por qué añadir más controles jerárquicos a un sistema rápido solo acelera su destrucción.
* **Meadows, D. H. (2008).** "Thinking in Systems: A Primer". Chelsea Green Publishing. [[Ver Libro]](https://www.amazon.com/Thinking-Systems-Donella-H-Meadows/dp/1603580557)
    * **Por qué leerlo:** La biblia de la dinámica de sistemas. Fundamental para entender el concepto de **Latencia Relativa**. Demuestra matemáticamente cómo los retrasos en la toma de decisiones (feedback loops diferidos) provocan inestabilidad terminal y por qué el control debe operar a la misma velocidad que el sistema.

### Bloque 2: La Arquitectura del Sacrificio (Antifragilidad y Fricción)

* **Taleb, N. N. (2012).** "Antifragile: Things That Gain from Disorder". Random House. [[Ver Libro]](https://www.amazon.com/Antifragile-Things-That-Gain-Disorder/dp/1400067820)
    * **Por qué leerlo:** Destruye la obsesión corporativa por la "robustez" y la predicción. Provee la base doctrinal para el **Sacrificio Programado** y los Nodos Críticos. Enseña que un sistema solo sobrevive si expone sus partes a la fricción local para proteger el núcleo global.
* **Snowden, D. J., & Boone, M. E. (2007).** "A Leader's Framework for Decision Making" (Cynefin). Harvard Business Review. [[Ver Documento]](https://hbr.org/2007/11/a-leaders-framework-for-decision-making)
    * **Por qué leerlo:** El marco Cynefin diferencia entre ecosistemas "Complicados" (donde funcionan los manuales y matrices) y "Complejos" (donde funciona nuestra Física Organizacional). Destruye la pretensión fiduciaria de gobernar la complejidad mediante "mejores prácticas" predictivas.

### Bloque 3: El Diseño de Contención (Cortocircuitos e Interfaces)

* **Nygard, M. (2018).** "Release It!: Design and Deploy Production-Ready Software". Pragmatic Bookshelf. [[Ver Libro]](https://www.amazon.com/Release-Design-Deploy-Production-Ready-Software/dp/1680502395)
    * **Por qué leerlo:** El manual técnico definitivo para la contención de daños. De aquí nace la implementación literal de los **Circuit Breakers (Cortocircuitos)**, **Bulkheads (Compartimentos Estancos)** y la **Degradación Elegante**. Traduce el concepto de supervivencia a patrones arquitectónicos exactos para reducir el $T_c$.
* **Beer, S. (1972).** "Brain of the Firm: The Managerial Cybernetics of Organization". Allen Lane. [[Ver Libro]](https://www.amazon.com/Managerial-cybernetics-organization-Stafford-1981-02-04/dp/B019TM5RWK)
    * **Por qué leerlo:** La obra maestra de la cibernética organizacional y el Modelo de Sistema Viable (VSM). Provee el sustento de la **Ley de Imputabilidad Estructural**, demostrando que un nivel jerárquico no puede controlar un sistema si no posee la "variedad" (capacidad de procesamiento y velocidad) necesaria para absorber las perturbaciones de la red.

### Bloque 4: La Certeza Balística (SRE y Pruebas de Estrés)

* **Rosenthal, C., & Jones, N. (2020).** "Chaos Engineering: System Resiliency in Practice". O'Reilly Media. [[Ver Libro]](https://www.amazon.com/Chaos-Engineering-System-Resiliency-Practice/dp/1492043869)
    * **Por qué leerlo:** La justificación empírica contra el "teatro de seguridad". Establece el protocolo para inyectar fricción deliberada en producción y medir empíricamente el Tiempo de Propagación ($T_p$). Si no inyectas caos para probar tus cortocircuitos, estás operando a ciegas.
* **Beyer, B., et al. (2016).** "Site Reliability Engineering (SRE)". O'Reilly Media. [[Ver Libro]](https://www.amazon.com/Site-Reliability-Engineering-Production-Systems/dp/149192912X)
    * **Por qué leerlo:** La doctrina operativa que materializa la inecuación de control. Transforma el cumplimiento normativo abstracto en *Service Level Objectives* (SLOs), estableciendo las **Envolventes de Viabilidad** matemáticas y fundamentando al SRE como una función distribuida con autoridad para detener la red cuando se cruza el límite.

### Bloque 5: La Viabilidad Estructural (Adaptación y Envolventes)

* **Ashby, W. R. (1956).** "An Introduction to Cybernetics". Chapman & Hall. [[Ver Libro]](https://www.amazon.com/Introduction-Cybernetics-W-Ross-Ashby/dp/1614277656/)
    * **Por qué leerlo:** La formulación matemática de la **Ley de la Variedad Requerida** ("Solo la variedad absorbe variedad"). Es la prueba científica de por qué un directorio con controles lentos no puede gobernar un sistema rápido. Si la arquitectura de control (SRE/Cortocircuitos) no tiene la misma complejidad y velocidad que la amenaza, el sistema colapsa por déficit estructural.
* **Dekker, S. (2011).** "Drift into Failure: From Hunting Broken Components to Understanding Complex Systems". Ashgate. [[Ver Libro]](https://www.amazon.com/Drift-into-Failure-Components-Understanding/dp/1409422216)
    * **Por qué leerlo:** Demuestra forensemente cómo los sistemas caen en la "deriva hacia el fallo" justificando pequeñas excepciones operativas (nuestro concepto de *Interacciones Huérfanas*). Destruye por completo el Análisis de Causa Raíz (RCA) tradicional y justifica la necesidad imperiosa de las **Envolventes de Viabilidad**.

### Bloque 6: El Motor de Implementación (SRE y Bucle de Adaptación)

* **Forsgren, N., Humble, J., & Kim, G. (2018).** "Accelerate: The Science of Lean Software and DevOps". IT Revolution Press. [[Ver Libro]](https://www.amazon.com/Accelerate-Software-Performing-Technology-Organizations/dp/1942788339)
    * **Por qué leerlo:** Provee la evidencia estadística y científica para sostener la **Gobernanza Bimodal**. Demuestra que la velocidad de operación y la estabilidad (riesgo) no son un juego de suma cero. La inyección de políticas en el código (Compliance as Code) es lo único que permite gobernar sin ser el cuello de botella.
* **Woods, D. D., et al. (2015).** "Resilience Engineering in Practice: A Guidebook". Ashgate. [[Ver Libro]](https://www.amazon.com/Resilience-Engineering-Practice-Guidebook-Ashgate/dp/1472420748)
    * **Por qué leerlo:** El manual definitivo sobre cómo sostener el **Bucle de Adaptación Continua**. Explica cómo las organizaciones deben cambiar su postura de "respuesta a incidentes" a una postura de "monitoreo de la tensión de la red", justificando la eliminación de los KPIs divisionales que fomentan la optimización local destructiva.