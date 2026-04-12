# ANEXO G: Protocolo de Implementación Sistémica (12 Meses)

El rediseño organizacional no se evangeliza; se instala. El cambio hacia una gobernanza bajo incertidumbre no es un proyecto de gestión cultural, sino una migración de infraestructura operativa que debe ejecutarse con el motor de la organización en marcha. 

La implementación no falla por complejidad técnica. Falla cuando la organización intenta preservar sus métricas heredadas. El sistema no se instala cuando se entiende. Se instala cuando reemplaza mecánicamente los procesos anteriores.

Este protocolo define la arquitectura de despliegue en cuatro fases ineludibles. Su objetivo es instalar un Modelo Operativo Mínimo Viable (MVP Sistémico) en el plazo de un año, reemplazando el control lineal por gobernanza geométrica. 

**Regla de Transición:** Ninguna fase puede iniciarse si el hito auditable de la fase anterior no ha sido cumplido empíricamente. La transición no es cronológica. Es condicional. Si un hito auditable no puede demostrarse de forma empírica, la fase no se considera incompleta. Se considera fallida y debe ser reiniciada.

---

### FASE 1 — INSTRUMENTACIÓN (Meses 1 al 3)

**Objetivo:** Cartografía de interfaces críticas y despliegue de la capa de observabilidad.

La transición comienza asumiendo la ceguera actual del sistema. Antes de gobernar, la arquitectura debe ser capaz de ver la fricción.

* **Delimitación del perímetro:** Selección quirúrgica de las tres interfaces transversales con mayor densidad de riesgo (por asimetría de consecuencia, opacidad algorítmica o volumen). El perímetro MVP opera como un entorno controlado donde el modelo lineal queda suspendido. Fuera de este perímetro, la organización continúa bajo el modelo heredado.
* **Despliegue de sensores forenses:** Instalación de telemetría dura en el perímetro MVP (monitoreo de APIs, medición de excepciones manuales y captura de latencia de procesamiento).
* **Pureza de la Capa de Observabilidad:** Ingesta de todos los eventos del perímetro hacia un repositorio inmutable y correlacionado. La capa de observabilidad no puede depender de datos interpretados o agregados manualmente. Solo se consideran válidos los eventos generados directamente desde la capa de ejecución.
* **HITO AUDITABLE:** *El sistema es capaz de demostrar en tiempo real la latencia y la tasa de fricción exacta entre las tres áreas seleccionadas, sin depender de reportes, encuestas ni testimonios humanos.*

---

### FASE 2 — PARAMETRIZACIÓN (Meses 4 al 6)

**Objetivo:** Compilación de contratos de acoplamiento y definición de las envolventes de viabilidad.

Una vez que la fricción es visible, se establecen los límites matemáticos de la autonomía operativa.

* **Traducción de políticas a código:** Las restricciones operativas, financieras y de cumplimiento de las interfaces seleccionadas se compilan como parámetros físicos.
* **Diseño de la envolvente MVP:** Establecimiento de los umbrales de tolerancia geométrica (tiempos de respuesta máximos, presupuestos de error, formatos de datos inquebrantables). Ningún parámetro definido en la envolvente de viabilidad puede ser sobreescrito manualmente por la operación. Toda excepción debe ser codificada o rechazada.
* **Codificación del escalamiento:** Formalización del Protocolo de Escalamiento Sistémico (Nivel 1: Degradación elegante; Nivel 2: Intervención SRE; Nivel 3: Sacrificio irreversible predefinido).
* **HITO AUDITABLE:** *La arquitectura bloquea físicamente cualquier transacción en la interfaz que intente perforar la envolvente de viabilidad, sin requerir la intervención de un supervisor.*

---

### FASE 3 — TRANSFERENCIA DE CONTROL (Meses 7 al 9)

**Objetivo:** Destrucción del control *ex post* e instalación de la Ingeniería de Confiabilidad del Sistema (SRE Corporativo).

La validación de la arquitectura transfiere el poder desde la jerarquía hacia la topología.

* **Mutación de la línea de defensa:** El área de auditoría interna abandona el muestreo forense de transacciones pasadas y asume el rol de SRE Corporativo.
* **Prohibición de coexistencia:** El control *ex post* y el control embebido no pueden coexistir sobre la misma interfaz. La coexistencia introduce ambigüedad y degrada ambos modelos. 
* **Nuevo checklist operacional:** El SRE comienza a auditar exclusivamente el código de los *circuit breakers*, la inmutabilidad de los *logs* en la Capa de Observabilidad y la vigencia de los contratos de acoplamiento.
* **Activación de métricas topológicas:** Se encadenan los incentivos y se penaliza la externalización del riesgo. La eliminación de KPIs divisionales no es una decisión organizacional. Es una consecuencia matemática de la imposibilidad de medir el sistema mediante nodos aislados.
* **HITO AUDITABLE:** *Eliminación formal de los KPIs divisionales en el perímetro intervenido. La evidencia inmutable generada por el sistema reemplaza legalmente al control de firmas y validaciones manuales.*

---

### FASE 4 — AUTONOMÍA ADAPTATIVA (Meses 10 al 12)

**Objetivo:** Encendido del bucle de adaptación y apagado definitivo del modelo lineal en las interfaces críticas.

La máquina comienza a respirar de forma autónoma, utilizando la fricción termodinámica como combustible para auto-calibrarse.

* **Traspaso de autoridad táctica:** El vértice estratégico cede formalmente la autoridad de decisión operativa a la frontera, sujeta estrictamente a los límites de la envolvente.
* **Respiración sistémica:** Habilitación de la lógica de expansión y contracción automática. El sistema reajusta el tamaño de sus envolventes basándose en la telemetría de latencia en tiempo real. El bucle de adaptación debe operar dentro de límites de seguridad predefinidos. Una recalibración fuera de esos límites no optimiza el sistema; lo desestabiliza. El bucle de adaptación no perdona errores de parametrización.
* **Inyección de estrés (Testeo):** Ejecución de simulacros de caos controlado para validar la respuesta de la jerarquía de intervención geométrica.
* **HITO AUDITABLE:** *El sistema absorbe un evento sistémico de alta fricción, degrada sus servicios no críticos automáticamente (Nivel 1) y protege la continuidad operativa sin requerir la convocatoria de un comité de crisis.*

---

**ESTADO FINAL DEL DESPLIEGUE**

Al concluir el Mes 12, la organización ya no depende de la capacidad de sus directivos para sobrevivir. Depende de su arquitectura. 

Una vez que una interfaz ha sido absorbida por la arquitectura sistémica, no puede volver al modelo lineal sin introducir un riesgo estructural inmediato. A partir del Mes 13, la infraestructura no requiere ser rediseñada; simplemente se escala topológicamente, repitiendo el protocolo para devorar las siguientes interfaces críticas del organigrama hasta que el modelo lineal quede obsoleto por inanición.

La organización no se transforma cuando adopta un modelo. Se transforma cuando ya no puede operar sin él. La arquitectura no se adopta. Se impone por la imposibilidad física de sobrevivir fuera de sus límites.