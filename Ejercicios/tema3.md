
# TEMA 3: Ejercicios:


1. **Buscar con qué órdenes de terminal o herramientas gráficas podemos configurar bajo Windows y bajo Linux el enrutamiento del tráfico de un servidor para pasar el tráfico desde una subred a otra**


En Windows se puede hacer sobre una interfaz, en Linux con los siguientes comandos:

```bash
	ip route [ip red destino][mascara de subred][ip siguiente salto]
```

Windows:

```bash
	Route ADD 192.168.136.218 MASK 255.255.255.255 192.168.136.1
```



2. **Buscar con qué órdenes de terminal o herramientas gráficas podemos configurar bajo Windows y bajo Linux el filtrado y bloqueo de paquetes**


En Linux tenemos la herramienta iptables, que cuenta con multitud de opciones y nos ofrece la posibilidad de construir múltiples reglas para afinar el filtrado a nuestras necesidades.

En Windows puede conseguirse el filtrado de paquetes a través de la interfaz de Windows Small Business Server 2003 o Windows Server 2003 o bien con cualquier firewall.
