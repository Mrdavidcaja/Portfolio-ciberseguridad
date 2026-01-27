# SOC Lab (Simulado)

## 1. Objetivo
Simular el funcionamiento de un SOC (Security Operations Center) para demostrar conocimientos básicos de detección y respuesta a incidentes.

## 2. Flujo SOC
1. **Monitorización**
2. **Detección**
3. **Investigación**
4. **Contención**
5. **Erradicación**
6. **Recuperación**
7. **Lecciones aprendidas**

## 3. Herramientas (básicas)
- Splunk (para logs y dashboards)
- Wireshark (análisis de red)
- Sysmon (logs Windows)
- Zeek (análisis de tráfico)
- ELK (opcional)

## 4. Caso práctico (ejemplo)
### Alerta: múltiples intentos de login fallidos

**Datos del incidente:**
- IP: 192.168.1.10
- Usuario: admin
- Evento: 5 fallos de login en 2 minutos

**Acciones:**
1. Confirmar si es un ataque real.
2. Bloquear IP en firewall o en endpoint.
3. Cambiar contraseña si es necesario.
4. Revisar logs adicionales.
5. Reporte del incidente.

## 5. Resultado esperado
- Detectar patrón de brute force
- Generar alerta
- Contener el incidente
- Documentar en informe

