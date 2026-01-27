SOC Lab (Simulado) 
1. Objetivo

Simular el funcionamiento de un SOC (Security Operations Center) para demostrar conocimientos básicos de detección, análisis y respuesta ante incidentes.

2. Flujo SOC

Monitorización

Detección

Investigación

Contención

Erradicación

Recuperación

Lecciones aprendidas

3. Herramientas (básicas)

Splunk (para logs y dashboards)

Wireshark (análisis de red)

Nmap (escaneo de red básico)

Herramientas Windows/Linux básicas (Event Viewer, logs, cmd, terminal)

Firewall / IPS (bloqueo de tráfico)

Endpoint (EDR básico)

4. Caso práctico (ejemplo)

Alerta: tráfico anómalo saliente a una IP externa desconocida (posible exfiltración).

Datos del incidente:

Origen: 192.168.1.25

Destino: 45.77.120.88

Protocolo: HTTPS (443)

Volumen: 2 GB en 15 minutos

Proceso: chrome.exe (o navegador)

Usuario: usuario1

Acciones (paso a paso):

1. Confirmar si es actividad maliciosa

Revisar logs de firewall y proxy.

Analizar el destino (IP/URL) con herramientas de reputación.

Verificar si hay correlación con otros eventos (picos, alertas, otros equipos).

2. Investigar el origen

Revisar logs del endpoint (EDR).

Buscar procesos sospechosos o inusuales.

Comprobar si hay cambios en archivos o conexiones persistentes.

3. Contención

Bloquear la IP externa en firewall o proxy.

Aislar el equipo afectado en la red (segmentación o cuarentena).

Finalizar procesos sospechosos en el endpoint.

4. Erradicación

Eliminar malware o scripts detectados.

Revisar y eliminar persistencias (tareas programadas, servicios, startup).

Actualizar antivirus/EDR y ejecutar análisis completo.

5. Recuperación

Restaurar el equipo afectado a un estado seguro.

Revisar permisos de usuario y credenciales.

Aplicar parches o medidas correctivas.

6. Lecciones aprendidas

Revisar por qué no se detectó antes.

Mejorar reglas en Splunk/IPS.

Mejorar segmentación de red o políticas de proxy.

5. Resultado esperado

Detectar tráfico anómalo saliente (posible exfiltración).

Generar alerta y escalar si es necesario.

Contener el incidente bloqueando la IP y aislando el equipo.

Documentar todo el proceso en un informe.
