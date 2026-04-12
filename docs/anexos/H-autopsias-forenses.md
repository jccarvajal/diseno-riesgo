# Anexo H: Autopsias Forenses Comparadas
### El Contraste entre el Teatro Documental y la Física Organizacional

La teoría no sobrevive al contacto con el enemigo. Este anexo desclasifica siete escenarios de colapso sistémico arquetípicos, demostrando empíricamente por qué los controles tradicionales fracasan frente a la velocidad de la red y cómo la implementación de la inecuación $T_p < T_c$ habría garantizado la supervivencia.

---

### Autopsia 1: El Contagio Transversal (Ransomware en Entornos Regulados)

**El Contexto:** Una agencia de fiscalización gubernamental sufre un ataque de ransomware (ej. variante Akira). El malware ingresa por una vulnerabilidad en la red administrativa de recursos humanos y, debido al acoplamiento de la red, salta a los servidores centrales que almacenan la evidencia de las inspecciones y auditorías de las entidades reguladas.

* **El Teatro Documental (Cómo se gestionó):** El mapa de calor mostraba el riesgo de ciberseguridad en "verde" porque existían políticas de contraseñas y antivirus instalados. Al detectarse la intrusión, el protocolo exigió convocar al comité de crisis TI. 
    * **El Resultado:** La latencia humana ($T_c$ de 4 horas) fue inútil contra un script de encriptación que viaja en milisegundos ($T_p$). Pérdida total de la evidencia forense.
* **La Solución Paramétrica (Diseño del Riesgo):** * **Identificación del Nodo Crítico:** Los repositorios de evidencia de fiscalización.
    * **El Cortocircuito ($T_c$):** Reglas de infraestructura como código (IaC) en la interfaz entre la red administrativa y la red de evidencia. Al detectar un patrón de cifrado anómalo o un pico de CPU, el *circuit breaker* aísla la subred de fiscalización de forma determinística en sub-segundos, sin intervención humana.
    * **El Sacrificio:** Se pierde la red administrativa (Fallo Absorbible), pero la capacidad sancionatoria del Estado (Nodo Crítico) sobrevive.

---

### Autopsia 2: La Falla de Interdependencia (Caída de API de Terceros)

**El Contexto:** Un banco digital integra una API de un proveedor externo para la validación de identidad (KYC). El proveedor sufre una degradación silente (sus servidores no caen, pero responden con 45 segundos de retraso).

* **El Teatro Documental:** El SLA del proveedor dice 99.9% de *uptime*. Como los servidores no están "caídos", las alarmas tradicionales de monitoreo no saltan. Las colas de conexión del banco se saturan esperando la respuesta del proveedor.
    * **El Resultado:** Efecto cascada. La saturación de la API de validación tumba el motor transaccional completo. Nadie en el banco puede transferir dinero.
* **La Solución Paramétrica:**
    * **Identificación del Nodo Crítico:** El motor transaccional primario.
    * **El Cortocircuito ($T_c$):** Implementación de un patrón *Circuit Breaker* en la arquitectura de software. Si la latencia del proveedor externo supera los 2 segundos, el circuito se "abre" automáticamente.
    * **El Sacrificio:** Durante 3 horas, no se pueden registrar clientes nuevos (Fallo Absorbible), pero los millones de clientes existentes siguen operando con normalidad (Supervivencia del Core). 

---

### Autopsia 3: La Aceleración del Pánico (Fuga de Liquidez Digital)

**El Contexto:** Un rumor en redes sociales desata un pánico bancario en una plataforma de inversiones. Los clientes comienzan a retirar sus fondos masivamente a través de la aplicación móvil.

* **El Teatro Documental:** El banco tiene un "Comité de Riesgo de Liquidez" que se reúne semanalmente y un BCP (Plan de Continuidad) diseñado para sucursales físicas. Las transferencias digitales operan sin fricción.
    * **El Resultado:** El dinero sale a velocidad de máquina. Cuando el directorio logra reunirse de emergencia 12 horas después, la institución ya está técnicamente insolvente.
* **La Solución Paramétrica:**
    * **Identificación del Nodo Crítico:** La reserva fraccionaria legal mínima.
    * **El Cortocircuito ($T_c$):** Un *Rate Limiter* algorítmico atado a las reservas de liquidez. Si la velocidad de salida de capital cruza el Límite Crítico de Acoplamiento, el sistema inyecta "fricción programada" (por ejemplo, retrasando las transferencias no urgentes o limitando los montos máximos por segundo) de forma automática.
    * **El Sacrificio:** Se sacrifica la "experiencia de usuario" y la promesa de transferencias instantáneas (Fallo Absorbible), garantizando la solvencia estructural de la institución frente al regulador (Supervivencia del Core).

---

### Autopsia 4: El Flash Crash Algorítmico (Mercados Financieros)

**El Contexto:** Un algoritmo de trading de alta frecuencia (HFT) entra en un bucle de retroalimentación negativa debido a un error de redondeo. Comienza a vender activos de forma masiva, arrastrando los precios hacia abajo en microsegundos.

* **El Teatro Documental:** La política de inversión prohíbe ventas que superen el 5% de volatilidad diaria. Existe un "Comité de Vigilancia" que recibe alertas por correo electrónico.
    * **El Resultado:** Para cuando el oficial de cumplimiento abrió el correo, el mercado había borrado 500 millones de dólares en valoración. La latencia humana fue de 15 minutos ($T_c$); la propagación fue de 200 microsegundos ($T_p$).
* **La Solución Paramétrica:**
    * **Identificación del Nodo Crítico:** La reserva mínima de capital operativo.
    * **El Cortocircuito ($T_c$):** Un "Kill Switch" determinístico integrado en la capa de red del broker. Si el precio cae un 2% en una ventana de 10 milisegundos, el sistema deniega físicamente cualquier orden de salida adicional.
    * **El Sacrificio:** Se pierde la oportunidad de "salir del mercado" a tiempo (Fallo Absorbible), pero se evita la quiebra técnica (Supervivencia del Core).

---

### Autopsia 5: El Efecto Látigo en Suministros (Logística Just-in-Time)

**El Contexto:** Una huelga en un puerto clave retrasa la entrega de un componente electrónico de 2 dólares. La empresa opera bajo un modelo de "eficiencia extrema" con stock cero.

* **El Teatro Documental:** El KPI es "Eficiencia de Inventario". El riesgo se gestiona pidiendo pólizas de seguro a los proveedores y firmando contratos con multas por retraso.
    * **El Resultado:** El seguro no fabrica microchips. El retraso de 2 dólares detiene una línea de montaje de productos de 2.000 dólares. El contagio atraviesa toda la cadena de producción por falta de buffers físicos.
* **La Solución Paramétrica:**
    * **Identificación del Nodo Crítico:** El cumplimiento del contrato con el cliente final.
    * **El Cortocircuito ($T_c$):** Redefinición de los límites de viabilidad. Si la telemetría del puerto indica un retraso mayor a $T_p$ (tiempo para que el stock llegue a cero), el sistema dispara una compra automática a un proveedor secundario (aunque sea más caro) o activa un "stock de sacrificio" precalculado.
    * **El Sacrificio:** Se acepta un mayor costo unitario y se rompe el KPI de eficiencia de inventario (Fallo Absorbible), para no pagar las multas millonarias por incumplimiento de entrega final (Nodo Crítico).

---

### Autopsia 6: La Cascada de Inestabilidad (Redes de Energía / Infraestructura)

**El Contexto:** Un exceso de demanda en un nodo de la red eléctrica provoca una caída de frecuencia. El sistema intenta compensar redistribuyendo la carga, pero esto sobrecarga los nodos vecinos.

* **El Teatro Documental:** Manuales de procedimientos de despacho de energía. Operadores humanos monitoreando pantallas y esperando órdenes de la central de control.
    * **El Resultado:** El "contagio" de sobrecarga viaja a la velocidad de la luz. El operador no tiene tiempo ni de levantar el teléfono. Un apagón regional total en 3 minutos.
* **La Solución Paramétrica:**
    * **Identificación del Nodo Crítico:** La integridad física de los transformadores centrales.
    * **El Cortocircuito ($T_c$):** Relés de protección de baja frecuencia automatizados. Al detectar una desviación paramétrica del 1%, el relé desconecta físicamente el área afectada antes de que la inestabilidad se propague.
    * **El Sacrificio:** Un barrio se queda a oscuras (Fallo Absorbible), protegiendo la red nacional de un colapso terminal que tardaría semanas en repararse.

---

### Autopsia 7: La Exfiltración de Datos Masiva (Privacidad y GRC)

**El Contexto:** Un error en la configuración de un bucket de almacenamiento en la nube deja expuestos 10 millones de registros de clientes. Un bot de rastreo detecta la vulnerabilidad y comienza la descarga masiva.

* **El Teatro Documental:** Auditoría de seguridad anual basada en cuestionarios (ISO 27001). Políticas de privacidad firmadas por todos los empleados.
    * **El Resultado:** El auditor no revisó la configuración de AWS porque "no estaba en la muestra". La empresa se entera 3 meses después por una filtración en prensa. Multa regulatoria terminal.
* **La Solución Paramétrica:**
    * **Identificación del Nodo Crítico:** La licencia para operar (cumplimiento de protección de datos).
    * **El Cortocircuito ($T_c$):** *Compliance as Code*. Un agente de seguridad automatizado monitorea las APIs de configuración. Si detecta un bucket público con datos sensibles, revoca los permisos de forma inmediata y bloquea el tráfico de salida.
    * **El Sacrificio:** Un desarrollador no puede acceder a sus archivos de prueba durante una hora (Fallo Absorbible), evitando la revocación de la licencia bancaria por negligencia grave (Nodo Crítico).