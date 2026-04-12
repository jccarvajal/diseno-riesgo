# ANEXO A: Modelo de Diagnóstico de Complejidad Organizacional

El diagnóstico de la complejidad no es una auditoría de cumplimiento regulatorio ni una evaluación de madurez cultural. Es un levantamiento topológico. Su propósito es medir, con precisión forense, el déficit de variedad entre la arquitectura de control de la organización y el entorno fuertemente acoplado en el que opera.

---

### REGLAS FUNDACIONALES DE VALIDEZ

El modelo opera bajo condiciones estrictas que prohíben el autoengaño corporativo:

1. **Principio Binario de Evidencia:** Si una capacidad sistémica no puede ser demostrada empíricamente mediante telemetría inmutable o evidencia paramétrica, se asume que no existe operativamente. La percepción de control por parte de la alta dirección se descarta como ruido.
2. **Regla de Invalidación Estructural:** Si alguna de las dimensiones de este modelo no puede ser evaluada mediante evidencia empírica directa, el diagnóstico completo se considera inválido. No existen los diagnósticos de resiliencia "parciales".
3. **Condición de Caducidad Termodinámica:** El diagnóstico pierde validez instantáneamente cuando la arquitectura del sistema (procesos o tecnología) cambia sin que la telemetría haya sido recalibrada. La vigencia del diagnóstico es función de la estabilidad topológica del sistema, no del tiempo cronológico transcurrido.

---

### DIMENSIÓN I: Topología de la Interfaz y Ceguera Estructural

Esta dimensión determina si la organización gobierna sus interacciones o simplemente administra el aislamiento de sus nodos funcionales.

**Axioma de la Dimensión:** *Una interfaz sin contrato de acoplamiento paramétrico no es una interfaz gobernada. Es un punto de falla no controlado.*

* **Identidad de la Interfaz:** ¿Están mapeados los puntos exactos donde el *output* de un dominio funcional se convierte en el *input* de otro?
    * *Criterio de fallo explícito:* Las interfaces se definen por acuerdos de nivel de servicio (SLAs) estáticos basados en tiempo, no por contratos de acoplamiento paramétricos basados en volumen de fricción y latencia geométrica.
* **Propiedad del Riesgo Intersticial:** Cuando una anomalía ocurre en el tránsito entre dos sistemas o departamentos, ¿existe una jurisdicción automatizada que absorba el evento?
    * *Criterio de fallo explícito:* El riesgo es disputado políticamente *post-mortem* o resuelto mediante excepciones manuales indocumentadas en la periferia táctica.
* **Telemetría Transversal:** ¿La organización mide la tasa de rechazo y la degradación inducida entre áreas?
    * *Criterio de fallo explícito:* Los tableros de control directivo muestran únicamente Indicadores Clave de Desempeño (KPIs) divisionales, asumiendo erróneamente que la suma de nodos en "verde" equivale a un sistema estable.

---

### DIMENSIÓN II: Asimetría Temporal y Velocidad de Intervención

Evalúa si la arquitectura de gobernanza posee la velocidad termodinámica necesaria para interceptar una cascada antes de que el daño sea irreversible.

**Axioma de la Dimensión:** *Un sistema es ingobernable cuando la latencia de decisión excede la velocidad de propagación del evento.*

* **Latencia de Decisión:** ¿Cuál es el tiempo que transcurre entre la detección algorítmica o táctica de una desviación crítica y la autorización formal para ejecutar una medida de contención sistémica?
    * *Criterio de fallo explícito:* La latencia de la decisión directiva (horas o días) es superior a la velocidad de propagación técnica o legal del evento (milisegundos). El control es estructuralmente extemporáneo.
* **Control Embebido vs. Diferido:** ¿Las restricciones operativas, legales y de seguridad están programadas como límites duros en el código del proceso transaccional?
    * *Criterio de fallo explícito:* El cumplimiento normativo se certifica mediante revisiones *ex post* o auditorías de muestreo aleatorio. La desviación ya se ha materializado en la red.
* **Proporcionalidad de la Reacción:** Ante un fallo en un componente, ¿el sistema puede desacoplarse temporalmente a velocidad de máquina?
    * *Criterio de fallo explícito:* El sistema prioriza la velocidad ininterrumpida sobre la contención, permitiendo que la automatización ciega amplifique el daño al ejecutar procesos correctos sobre premisas ya invalidadas.

---

### DIMENSIÓN III: Envolventes de Viabilidad y Autoridad Desplazada

Mide la capacidad de la organización para resolver el riesgo en la frontera, alineando el conocimiento táctico con la autoridad de ejecución.

**Axioma de la Dimensión:** *La autoridad centralizada sobre eventos que se propagan a velocidad de máquina es estructuralmente inefectiva.*

* **Autonomía Paramétrica:** ¿Tienen las interfaces periféricas el mandato técnico para rechazar operaciones o detener procesos si estos amenazan con perforar la tolerancia de diseño?
    * *Criterio de fallo explícito:* Toda desviación crítica requiere ser elevada por la jerarquía. El operador táctico no tiene autoridad técnica para detener la cascada, y la cúpula que tiene la autoridad carece del contexto para hacerlo con precisión.
* **Degradación Elegante:** Bajo estrés máximo, ¿sabe el sistema qué partes de su periferia debe sacrificar automáticamente para mantener la viabilidad de su núcleo?
    * *Criterio de fallo explícito:* Frente a la saturación, la organización colapsa uniformemente o depende de la improvisación humana bajo máxima presión temporal para decidir qué servicios apagar.
* **Asimetría de Consecuencia:** ¿El sistema de incentivos de un nodo funcional internaliza el costo de la fricción que le genera al nodo adyacente?
    * *Criterio de fallo explícito:* Un departamento puede alcanzar el 100% de cumplimiento de sus metas optimizando su operación local, mientras inyecta inestabilidad silenciosa en el resto de la red sin penalización paramétrica.

---

### DIMENSIÓN IV: Validación Empírica del Sistema (Stress Testing)

Determina si la organización opera basada en la fe en sus planes documentales o en la evidencia matemática de su resiliencia.

**Axioma de la Dimensión:** *Un sistema que no es sometido a perturbación controlada no puede demostrar su viabilidad. La ausencia de pruebas de estrés no indica estabilidad; indica falta de evidencia.*

* **Ingeniería de Fricción:** ¿La organización inyecta fallos y restricciones de manera deliberada en sus interfaces operativas para observar cómo se propaga la perturbación?
    * *Criterio de fallo explícito:* Las pruebas de estrés se limitan a simulacros lineales o *Disaster Recovery Plans* (DRPs) que evalúan la recuperación de componentes aislados, ignorando la dinámica del acoplamiento sistémico.
* **Auditabilidad de la Opacidad:** En procesos delegados a cajas negras (IA o algoritmos complejos), ¿existen *circuit breakers* que fuercen el retorno a la viabilidad si el modelo comienza a inferir fuera de los parámetros de riesgo aceptado?
    * *Criterio de fallo explícito:* La organización delega la ejecución de decisiones sin comprender la lógica probabilística, asumiendo pasivamente el riesgo generado por sistemas que no puede explicar ni detener a tiempo.

---

### VEREDICTO ARQUITECTÓNICO

La aplicación de este instrumento no produce un puntaje de riesgo. Produce un diagnóstico binario sobre la viabilidad de la infraestructura.

1.  **Déficit de Variedad Crítico:** Si el diagnóstico revela dependencia de SLAs estáticos, auditoría *ex post*, autoridad centralizada y ausencia de estrés inyectado, el control que la organización cree ejercer es una ilusión documentada. El colapso sistémico no es una probabilidad; es una latencia termodinámica a la espera de un detonador transversal.
2.  **Proporcionalidad Arquitectónica:** Si el diagnóstico evidencia contratos de acoplamiento paramétricos, control embebido, autonomía en envolventes y testeo forense continuo, la organización está equipada para gobernar bajo incertidumbre.

**El sistema no es tan seguro como indican sus controles. Es tan seguro como lo que su arquitectura es capaz de gobernar.**

**El control no se evalúa por lo que la organización ve. Se evalúa por lo que su arquitectura le permite ver.**