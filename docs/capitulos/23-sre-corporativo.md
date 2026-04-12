# CAPÍTULO 23: La mutación del control interno y el SRE corporativo

El modelo clásico de las "tres líneas de defensa" fue diseñado para un mundo donde el riesgo se materializaba a velocidad humana. Asume que la segunda y tercera línea pueden mitigar el daño revisando muestras aleatorias de transacciones pasadas. En ecosistemas hiperconectados, auditar el pasado no previene el futuro; solo documenta la autopsia de la red. 

Frente a la velocidad de propagación de un fallo transversal, la auditoría estática es estructuralmente irrelevante. Un área de control que revisa firmas en documentos PDF es un mecanismo de registro sin capacidad de intervención. La auditoría solo es válida si su latencia es inferior a la del evento que intenta gobernar. Si no cumple esta condición, deja de ser control y se convierte en documentación.

El problema nunca fue que la organización no cumpliera. Fue que el cumplimiento no estaba embebido en el sistema que ejecuta. Un control que puede ser evadido por la operación no es un control. Es una recomendación.

### 23.1. De auditores a Ingenieros de Confiabilidad Sistémica

La arquitectura adaptada exige que las áreas de control muten hacia una función de Ingeniería de Confiabilidad del Sistema (SRE corporativo). 

La auditoría no desaparece. Se desplaza desde la revisión de decisiones hacia la verificación del sistema que las hace inevitables. El auditor contemporáneo deja de perseguir excepciones humanas para auditar la arquitectura. Su función es verificar en tiempo real la integridad y continuidad de la telemetría, y que las transacciones fluyan estrictamente dentro de las envolventes paramétricas. El objetivo del control no es detectar fallos. Es hacerlos físicamente imposibles o inmediatamente contenibles.

La función SRE no es un nuevo silo de poder. No tiene autoridad para reinterpretar la operación. Solo puede verificar y forzar el cumplimiento de las restricciones ya definidas. Si el SRE decide, la arquitectura falló. No tiene discrecionalidad política; opera dentro de parámetros auditablemente definidos.

### 23.2. El nuevo checklist forense y la contención de la caja negra

Si el control se embebe en la ejecución, la metodología de inspección cambia de raíz. El nuevo *checklist* forense audita la indemnidad de las reglas geométricas:
* **Auditoría de código y contratos de acoplamiento:** Verificación de que los tiempos máximos de respuesta y las reglas en la interfaz no hayan sido relajados por la operación.
* **Revisión de logs inmutables:** Inspección de la Capa de Observabilidad. Todo evento crítico debe generar un registro inmutable, verificable criptográficamente y correlacionado con la decisión ejecutada. Si la decisión no puede ser reconstruida a partir del *log*, no ocurrió. La ausencia de evidencia no es una debilidad de registro. Es una violación de control.
* **Testeo de latencias inyectadas:** El área de SRE inyecta fricción deliberada en las interfaces para probar empíricamente la velocidad de reacción de la red.

Esta instrumentación es crítica frente a la proliferación de la Inteligencia Artificial. La opacidad de una caja negra no puede ser auditada con metodologías lineales. Un sistema opaco solo es legítimo si su comportamiento está contenido dentro de límites verificables. La explicabilidad no es obligatoria; la contención sí lo es. La auditoría exige la instalación de *circuit breakers*. Si la IA se desvía milimétricamente de la envolvente, el cortocircuito salta, aísla el modelo y revierte el sistema a un estado controlable.

### 23.3. Protocolo de Escalamiento Sistémico

Otorgar autonomía táctica en las envolventes de viabilidad resuelve la fricción diaria. Sin embargo, la arquitectura requiere definir qué ocurre cuando el impacto termodinámico rompe esos límites.

La gobernanza sistémica impone una jerarquía de intervención pre-calculada. Cada nivel se activa automáticamente cuando las métricas topológicas exceden umbrales predefinidos en la envolvente de viabilidad. No hay interpretación humana en la activación:

* **Nivel 1 (Fricción alta): Absorción local.** El sistema detecta una anomalía severa pero contenible. Ejecuta automáticamente la degradación elegante. Rechaza transacciones no críticas, reduce la velocidad en la interfaz y prioriza el flujo *core* para mantener la continuidad, sin intervención humana.
* **Nivel 2 (Ruptura de envolvente): Intervención SRE.** La fricción perfora el límite paramétrico. Se dispara una alerta a la capa de control. La intervención técnica reconfigura temporalmente el contrato de acoplamiento o aísla el nodo infectado para proteger la red general.
* **Nivel 3 (Riesgo sistémico crítico): Sacrificio irreversible predefinido.** El desacople técnico falla. La supervivencia de toda la organización está comprometida. Aquí interviene la alta dirección, pero el Nivel 3 no es una instancia de deliberación ejecutiva. Es la ejecución de un sacrificio predefinido (por ejemplo, desconectar un canal de ventas completo). En este nivel, la prioridad no es la continuidad operativa. Es la supervivencia del sistema. La decisión no se toma en la crisis; se ejecuta en la crisis.

### 23.4. La topología de la intervención

Este protocolo erradica la ambigüedad en el peor momento posible. Elimina la parálisis por análisis y reemplaza la deliberación política por la ejecución mecánica de un plan de supervivencia. 

El escalamiento no sigue jerarquía organizacional. Sigue geometría de impacto. El organigrama es irrelevante cuando la red se incendia; lo único que importa es la topología de la propagación y los cortafuegos arquitectónicos.

**Un sistema sin jerarquía de intervención geométrica no es resiliente. Es inestable.**