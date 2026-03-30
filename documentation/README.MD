# Nexus Plaza Cyber Audit: Scoping and Rules of Engagement

Este repositorio documenta la fase de planificación y determinación del alcance (Pre-Engagement) para una auditoría de seguridad integral de la infraestructura de Nexus Plaza. El proyecto se centra en la metodología de trabajo remoto seguro y la definición de límites operativos para proteger entornos de producción críticos.

## Resumen del Proyecto
[cite_start]Nexus Plaza es una empresa minorista en línea con sede en Houston que requiere una evaluación de seguridad tras incidentes de ransomware sufridos por competidores en su sector[cite: 31, 40, 45]. [cite_start]El objetivo principal es identificar vulnerabilidades en los sistemas de logística e inventario para garantizar la continuidad del negocio y la entrega rápida a los clientes[cite: 47, 48].

## Metodología de Acceso Remoto
Para garantizar la seguridad y el cumplimiento durante la ejecución remota, se establecieron los siguientes protocolos de conectividad:
* [cite_start]Conexión Segura: El acceso a los sistemas internos se realiza exclusivamente a través de túneles SSL o IPsec VPN[cite: 43].
* [cite_start]Segmentación de Pruebas: Se utiliza una VLAN aislada dentro del departamento de TI como punto de origen para todas las actividades de escaneo y explotación[cite: 57].
* [cite_start]Monitoreo de Seguridad: Las pruebas interactúan con firewalls locales e IDS integrados para evaluar la capacidad de detección y respuesta ante incidentes del cliente[cite: 58, 59].

## Alcance Técnico (Scoping)
* [cite_start]Activos Incluidos: Clústeres de servidores de Operaciones y Logística[cite: 49, 100].
* [cite_start]Rangos de Red: Segmentos IP 172.26.0.0/21 y 172.27.0.0/21[cite: 100].
* [cite_start]Aplicaciones Críticas: Pruebas sobre instancias de Microsoft SQL Server que soportan el control de inventario[cite: 51, 101].
* [cite_start]Ingeniería Social: Pruebas de phishing limitadas a una lista específica de direcciones de correo electrónico proporcionada por la empresa[cite: 76, 130].
* [cite_start]Exclusiones: Se omiten explícitamente los sistemas de soporte de Amazon, el clúster de administración y la red LAN corporativa[cite: 53, 105].

## Reglas de Participación (Rules of Engagement)
| Elemento | Protocolo Establecido |
| :--- | :--- |
| Modalidad | [cite_start]Ejecución 100% Remota vía VPN Corporativa[cite: 43]. |
| Ventanas de Tiempo | [cite_start]Pruebas intrusivas limitadas de Viernes a Domingo (02:00 - 06:00 AM)[cite: 72, 73]. |
| Entorno de Datos | [cite_start]Uso de sistemas de desarrollo espejo para pruebas de bases de datos de producción[cite: 64, 68]. |
| Comunicación | [cite_start]Teleconferencias e informes de actualización semanales con el Director de TI y gerentes de área[cite: 80, 81]. |

## Documentación Detallada
* [Hoja de Trabajo del Alcance (Scoping)](documentation/scoping-worksheet.md)
* [Reglas de Participación (RoE)](documentation/rules-of-engagement.md)

---
Este proyecto forma parte de mi portafolio profesional de Ciberseguridad, demostrando competencias en Gestión de Riesgos, Cumplimiento (GRC) y Planificación de Auditorías.
