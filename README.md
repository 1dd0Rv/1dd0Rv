## Roddy · SecDevOps

Plataforma, CI/CD e identidad para equipos que despliegan a diario. Con base sólida de backend: no escribo solo el pipeline, también el servicio que pasa por él.

Técnico Superior en ASIR · `1dd0rv@proton.me`

### Stack

**Plataforma y CI/CD**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![SonarCloud](https://img.shields.io/badge/SonarCloud-F3702A?style=for-the-badge&logo=sonarqubecloud&logoColor=white)
![Postman](https://img.shields.io/badge/Newman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1904DA?style=for-the-badge&logo=trivy&logoColor=white)

**Seguridad**

![Keycloak](https://img.shields.io/badge/Keycloak-008AAA?style=for-the-badge&logo=keycloak&logoColor=white)
![Kong](https://img.shields.io/badge/Kong-003459?style=for-the-badge&logo=kong&logoColor=white)
![Wazuh](https://img.shields.io/badge/Wazuh-2C3E50?style=for-the-badge)
![TheHive](https://img.shields.io/badge/TheHive-2C3E50?style=for-the-badge)
![Cortex](https://img.shields.io/badge/Cortex-2C3E50?style=for-the-badge)
![MISP](https://img.shields.io/badge/MISP-2C3E50?style=for-the-badge)
![Shuffle](https://img.shields.io/badge/Shuffle-2C3E50?style=for-the-badge)

**Backend**

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![OpenAPI](https://img.shields.io/badge/OpenAPI-6BA539?style=for-the-badge&logo=openapiinitiative&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=for-the-badge&logo=flyway&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)

*Arquitectura hexagonal · OpenAPI contract-first · Resilience4j · SSE · MapStruct*

**Cloud**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge)

*VPC · EC2 · RDS · EFS · Security Groups*

**Sistemas y virtualización**

![Arch Linux](https://img.shields.io/badge/Arch_Linux-1793D1?style=for-the-badge&logo=archlinux&logoColor=white)
![Debian](https://img.shields.io/badge/Debian-A81D33?style=for-the-badge&logo=debian&logoColor=white)
![Kali](https://img.shields.io/badge/Kali-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
![Red Hat](https://img.shields.io/badge/Red_Hat-EE0000?style=for-the-badge&logo=redhat&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows_Server-0078D6?style=for-the-badge)
![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=for-the-badge&logo=proxmox&logoColor=white)

*TCP/IP · DNS · DHCP · VLAN · Switching*

**Lenguajes**

![Java](https://img.shields.io/badge/Java_17/21-437291?style=for-the-badge&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

### Proyectos

**TARTIS Recon-AI** — plataforma de gestión de parking · *rol DevOps en un equipo de 15*

Multirepo de 5 microservicios Spring Boot con arquitectura hexagonal estricta y contrato OpenAPI primero. Mi parte es la plataforma: Kong como gateway y Keycloak como proveedor de identidad, RabbitMQ para la mensajería asíncrona, GitHub Actions con gate de cobertura al 90% y análisis SonarCloud, branch protection uniforme en los 7 repos, y el stack completo levantándose tanto en Docker Compose como en Kubernetes con manifiestos Kustomize. Tests de contrato con Newman en CI.

**[Infraestructura WordPress en AWS](https://github.com/1dd0Rv/SREI/tree/wdpss_aws)** — *proyecto de SREI*

VPC repartida en dos zonas de disponibilidad con subredes públicas y privadas: la base de datos queda aislada en la privada, sin ruta desde internet. EC2 Debian con LAMP y security groups por servicio, RDS MySQL como motor gestionado, y EFS montado por NFS para que `wp-content` sea compartido y la capa web pueda escalar horizontalmente.

**Homelab SOC** — *TFG de ASIR*

Stack de detección y respuesta sobre Proxmox: Wazuh como XDR, TheHive para gestión de casos, Cortex para el análisis automatizado de observables, MISP como fuente de inteligencia y Shuffle para orquestar los playbooks. El objetivo: que una alerta llegue a caso enriquecido sin intervención manual.
