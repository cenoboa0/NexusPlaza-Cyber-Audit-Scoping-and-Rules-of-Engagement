Nexus Plaza Cyber Audit: Scoping and Rules of Engagement
Este repositorio documenta la fase de planificación y determinación del alcance (Pre-Engagement) para una auditoría de seguridad integral de la infraestructura de Nexus Plaza. El proyecto se centra en la metodología de trabajo remoto seguro y la definición de límites operativos para proteger entornos de producción críticos.

Resumen del Proyecto
Nexus Plaza es una empresa minorista en línea con sede en Houston que requiere una evaluación de seguridad tras incidentes de ransomware sufridos por competidores en su sector. El objetivo principal es identificar vulnerabilidades en los sistemas de logística e inventario para garantizar la continuidad del negocio y la entrega rápida a los clientes.

Metodología de Acceso Remoto
Para garantizar la seguridad y el cumplimiento durante la ejecución remota, se establecieron los siguientes protocolos de conectividad:

Conexión Segura: El acceso a los sistemas internos se realiza exclusivamente a través de túneles SSL o IPsec VPN.
Segmentación de Pruebas: Se utiliza una VLAN aislada dentro del departamento de TI como punto de origen para todas las actividades de escaneo y explotación.
Monitoreo de Seguridad: Las pruebas interactúan con firewalls locales e IDS integrados para evaluar la capacidad de detección y respuesta ante incidentes del cliente.
Alcance Técnico (Scoping)
Activos Incluidos: Clústeres de servidores de Operaciones y Logística.
Rangos de Red: Segmentos IP 172.26.0.0/21 y 172.27.0.0/21.
Aplicaciones Críticas: Pruebas sobre instancias de Microsoft SQL Server que soportan el control de inventario.
Ingeniería Social: Pruebas de phishing limitadas a una lista específica de direcciones de correo electrónico proporcionada por la empresa.
Exclusiones: Se omiten explícitamente los sistemas de soporte de Amazon, el clúster de administración y la red LAN corporativa.
Reglas de Participación (Rules of Engagement)
Elemento	Protocolo Establecido
Modalidad	Ejecución 100% Remota vía VPN Corporativa.
Ventanas de Tiempo	Pruebas intrusivas limitadas de Viernes a Domingo de 02:00 a 06:00 AM.
Entorno de Datos	Uso de sistemas de desarrollo espejo para pruebas de bases de datos de producción.
Comunicación	Teleconferencias e informes de actualización semanales con el Director de TI y gerentes de área.
Documentación Detallada
Hoja de Trabajo del Alcance (Scoping)
Reglas de Participación (RoE)
Este proyecto forma parte de mi portafolio profesional de Ciberseguridad, demostrando competencias en Gestión de Riesgos, Cumplimiento (GRC) y Planificación de Auditorías.
