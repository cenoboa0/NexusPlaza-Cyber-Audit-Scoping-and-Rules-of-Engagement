# Hoja de Trabajo del Alcance: Nexus Plaza

Este documento detalla el análisis de alcance realizado tras la entrevista con el CEO y el Director de TI de Nexus Plaza para definir los límites de la auditoría de seguridad.

## 1. Preocupaciones de Seguridad del Cliente
La mayor preocupación es que los sistemas de inventario y envío sufran un ataque de ransomware. Una interrupción en estos procesos impediría cumplir con los pedidos a tiempo, lo cual sería crítico para la continuidad del negocio.

## 2. Activos y Rangos Incluidos (In-Scope)
Se deben probar los siguientes elementos críticos:
* Clústeres de Servidores: Operaciones y Logística.
* Rangos de Red: 172.26.0.0/21 y 172.27.0.0/21.
* Aplicaciones: Instancias de Microsoft SQL Server que soportan el sistema de inventario.

## 3. Activos Excluidos (Out-of-Scope)
Para evitar riesgos innecesarios o interferencias con servicios de terceros, se excluyen explícitamente:
* Clústeres de Administración y Soporte de Amazon.
* Todos los rangos de direcciones IP de la LAN corporativa.
* Acceso inalámbrico y servicios web externos alojados en Amazon.

## 4. Metodología de Acceso y Pruebas
* Entorno: La mayoría de las pruebas se realizarán en sistemas de producción. Las pruebas intrusivas de SQL Server se limitarán a un entorno de desarrollo configurado de forma idéntica con un espejo de la base de datos.
* Origen del Acceso: El acceso se realizará a través de una VLAN aislada dentro del departamento de TI proporcionada por el cliente.
* Ingeniería Social: Autorizada únicamente contra una lista limitada de direcciones de correo electrónico proporcionada por la empresa.
* Ataques Disruptivos: Permitidos, incluyendo ataques de denegación de servicio (DoS), solo durante las ventanas de mantenimiento programadas.

## 5. Ubicación Física
El centro de datos objeto de la auditoría se encuentra ubicado físicamente en las instalaciones de Houston.
