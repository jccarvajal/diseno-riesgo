# ANEXO B: Mapa de Interdependencias Críticas

El organigrama es una ficción administrativa que documenta la autoridad estática. El Mapa de Interdependencias Críticas es la cartografía topológica de la realidad operativa. Su objetivo no es registrar quién reporta a quién, sino revelar la geometría exacta por donde se propaga el daño sistémico.

Si el riesgo es una propiedad emergente de las interacciones (Capítulo 14), la organización no puede ser diagnosticada evaluando el estado de sus nodos funcionales. Este mapa ignora el desempeño local para medir exclusivamente la tensión termodinámica en las aristas (las interfaces) que conectan dichos nodos.

**Axioma de Obligatoriedad:** *Si la organización no puede mapear sus interfaces críticas bajo estos cuatro vectores, no posee capacidad estructural para gobernar el riesgo sistémico.*

---

### VECTORES DE CARTOGRAFÍA SISTÉMICA

#### VECTOR I: Delimitación Física de la Interfaz
La organización asume que las áreas interactúan de manera fluida. El mapa exige probar empíricamente dónde se rompe el flujo. Una interfaz crítica se mapea únicamente cuando se cumple al menos una de las siguientes tres condiciones de transferencia:
1.  **Transferencia de Jurisdicción:** El proceso cruza una frontera donde cambia la responsabilidad legal, financiera o de cumplimiento operativo (ej. de Ventas a Riesgos).
2.  **Asimetría de Frecuencia:** Un flujo que opera en tiempo real choca contra un dominio que opera en lotes o bajo tiempos humanos (ej. conciliación algorítmica vs. validación manual).
3.  **Mutación de Formato (Traducción):** El formato de los datos o el vocabulario operativo debe ser reinterpretado o transcrito para ser procesado por el nodo receptor.

*Regla de exclusión:* Si no hay cambio de jurisdicción, frecuencia o formato, no es una interfaz crítica. Es un proceso interno del nodo y queda fuera del alcance del mapa.

#### VECTOR II: Direccionalidad, Temporalidad y Asimetría
En ecosistemas acoplados, la dependencia rara vez es simétrica. El mapa no traza líneas bidireccionales genéricas; vectoriza la dirección y la velocidad del daño.
* **Vector de Consecuencia:** Se mapea topológicamente quién toma la decisión (Origen) y quién absorbe el impacto legal o financiero (Destino). Si el área Comercial decide acelerar el *onboarding* (Origen), pero Operaciones hereda el costo por datos incompletos (Destino), el vector se dibuja hacia Operaciones.
* **Tiempo de Colapso:** El vector debe incluir el tiempo de propagación del daño. *Una dependencia sin temporalidad medida no es gobernable.* Si el Nodo A se detiene, ¿cuántos milisegundos u horas transcurren antes de que el Nodo B se paralice por inanición?
*Regla de cartografía:* Toda interacción donde el origen de la decisión está desacoplado del destino de la consecuencia es catalogada inmediatamente como "Falla Geológica" de alto riesgo.

#### VECTOR III: Parametrización del Acoplamiento Actual
Para cada interfaz delimitada, el mapa extrae forensemente las condiciones de funcionamiento real, ignorando las declaraciones de cumplimiento. Se mapean tres parámetros duros:
1.  **Latencia Estructural:** El tiempo exacto que requiere el sistema para procesar la transferencia transversal y absorber sus fricciones. *Una interfaz se considera en estado de saturación cuando la latencia estructural supera el 80% de su tiempo de ciclo definido.*
2.  **Tasa de Excepciones Manuales:** El porcentaje del volumen transaccional que requiere un parche humano o la desactivación de un control automatizado para cruzar la frontera.
3.  **Tolerancia a la Degradación:** Si la interfaz sufre una perturbación, ¿posee un *buffer* (holgura) para absorber el impacto sin afectar el servicio final, o el acoplamiento es tan fuerte que la propagación es instantánea?

#### VECTOR IV: Identificación de Zonas Huérfanas (Opacidad)
El mapeo topológico expone los espacios de la red que no tienen gobierno explícito. Estas son las incubadoras del colapso sistémico.
* **Colisión de SLAs:** Intersecciones donde los Indicadores Clave de Desempeño (KPIs) del Nodo A entran en conflicto directo con las métricas de cumplimiento del Nodo B.
* **Riesgo No Asignado:** El mapa identifica vacíos jurisdiccionales donde la transferencia de un riesgo transversal no tiene un propietario técnico asignado en las envolventes de viabilidad.
*Regla de Inviabilidad:* *Toda zona huérfana identificada se clasifica automáticamente como punto de fallo crítico, independiente de su impacto observable actual.*

---

### RESULTADO: La Matriz Topológica

El entregable de este modelo no es un diagrama de flujo. Es una **Matriz Topológica de Red** que clasifica cada interfaz en uno de tres estados físicos:

1.  **Acoplamiento Estable:** La interfaz posee contratos de acoplamiento claros, autonomía periférica para degradarse y la fricción es absorbida dentro de la envolvente de viabilidad.
2.  **Acoplamiento Sobrecargado (Riesgo Latente):** La latencia estructural consume más del 80% del tiempo de ciclo. El sistema funciona, pero carece de la holgura termodinámica para absorber cualquier perturbación. Una desviación milimétrica iniciará una cascada.
3.  **Acoplamiento Roto (Ceguera):** Existen asimetrías de consecuencia severas, el conocimiento y la autoridad están separados, y la interfaz sobrevive exclusivamente mediante parches tácticos indocumentados.

**Axioma de Despliegue:** *El perímetro del Modelo Operativo Mínimo Viable (MVP) no se define por criticidad de negocio. Se define exclusivamente por las interfaces en estado de Acoplamiento Roto.* Estas dictan obligatoriamente el punto de intervención durante la Fase 1 del Protocolo de Implementación (Anexo F).

**Condición de Caducidad:** El mapa de interdependencias pierde validez cuando cambia la topología operativa sin recalibración de sus vectores.

**La organización no falla donde se controla. Falla donde no está mapeada.**