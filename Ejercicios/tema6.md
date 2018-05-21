
# TEMA 6: Ejercicios:


1. **Aplicar con iptables una política de denegar todo el tráfico en una de las máquinas de prácticas**


Bloquear todo el tráfico:

```bash
	iptables -F
	iptables -P INPUT DROP
	iptables -P OUTPUT DROP
	iptables -P FORWARD DROP
```


2. **Aplicar con iptables una política de permitir todo el tráfico en una de las máquinas de prácticas**

Permitir todo:

```bash
	iptables -F
	iptables -I INPUT -j ACCEPT
```



3. **Buscar información acerca de los tipos de ataques más comunes en servidores web (p.ej. secuestros de sesión). Detallar en qué consisten, y cómo se pueden evitar**


Ataque por injection: es una técnica para modificar una cadena de consulta de base de datos.

Ataques DDoS: consisten en inundar un sitio web con solicitudes externas. Para prevenirnos debemos implementar algún tipo de denegación de servicio, de forma que no nos sature el sistema.

Cross Site Scriptin: inyectan scripts maliciosos en sitios web inofensivos.



