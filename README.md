## Roddy · SecDevOps

Plataforma, CI/CD e identidad para equipos que despliegan a diario. Con base sólida de backend: no escribo solo el pipeline, también el servicio que pasa por él.

Técnico Superior en ASIR · `1dd0rv@proton.me`

### Stack

| Área | |
|---|---|
| **Plataforma y CI/CD** | Docker · Docker Compose · Kubernetes (minikube, Kustomize) · GitHub Actions · SonarCloud · Newman · Trivy |
| **Seguridad** | Keycloak (OIDC) · Kong (API Gateway) · Wazuh · TheHive · Cortex · MISP · Shuffle |
| **Backend** | Java 17/21 · Spring Boot · Arquitectura hexagonal · OpenAPI contract-first · Flyway · MapStruct · RabbitMQ · Resilience4j · SSE · PostgreSQL |
| **Cloud** | AWS — VPC · EC2 · RDS · EFS · Security Groups |
| **Sistemas y red** | Linux (Arch, Debian, Kali, RHEL) · Windows Server · Proxmox · TCP/IP · DNS · DHCP · VLAN |
| **Lenguajes** | Java · Python · Bash · TypeScript |

### Proyectos

**TARTIS Recon-AI** — plataforma de gestión de parking · *rol DevOps en un equipo de 15*

Multirepo de 5 microservicios Spring Boot con arquitectura hexagonal estricta y contrato OpenAPI primero. Mi parte es la plataforma: Kong como gateway y Keycloak como proveedor de identidad, RabbitMQ para la mensajería asíncrona, GitHub Actions con gate de cobertura al 90% y análisis SonarCloud, branch protection uniforme en los 7 repos, y el stack completo levantándose tanto en Docker Compose como en Kubernetes con manifiestos Kustomize. Tests de contrato con Newman en CI.

**[Infraestructura WordPress en AWS](https://github.com/1dd0Rv/SREI/tree/wdpss_aws)** — *proyecto de SREI*

VPC repartida en dos zonas de disponibilidad con subredes públicas y privadas: la base de datos queda aislada en la privada, sin ruta desde internet. EC2 Debian con LAMP y security groups por servicio, RDS MySQL como motor gestionado, y EFS montado por NFS para que `wp-content` sea compartido y la capa web pueda escalar horizontalmente.

**Homelab SOC** — *TFG de ASIR*

Stack de detección y respuesta sobre Proxmox: Wazuh como XDR, TheHive para gestión de casos, Cortex para el análisis automatizado de observables, MISP como fuente de inteligencia y Shuffle para orquestar los playbooks. El objetivo: que una alerta llegue a caso enriquecido sin intervención manual.
