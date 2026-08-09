```bash
$ whoami
> Roddy — SecDevOps. Técnico Superior en ASIR.
> Construyo la plataforma sobre la que corre el código: CI/CD, contenedores,
> identidad y observabilidad. Con bastante backend en las manos, no solo YAML.

$ cat focus.txt
> Seguridad y automatización dentro del ciclo de vida, no pegadas al final.
> Gateway + identidad, gates de calidad que bloquean de verdad,
> y entornos reproducibles de Compose a Kubernetes.
```

### Stack

**Plataforma y CI/CD**
`Docker` · `Docker Compose` · `Kubernetes (minikube, Kustomize)` · `GitHub Actions` · `SonarCloud` · `Newman/Postman` · `Trivy` · `Proxmox`

**Cloud**
`AWS (VPC, EC2, RDS, EFS, Security Groups)`

**Seguridad**
`Keycloak (OIDC)` · `Kong (API Gateway)` · `Wazuh` · `TheHive` · `Cortex` · `MISP` · `Shuffle`

**Backend**
`Java 17/21` · `Spring Boot` · `Arquitectura hexagonal` · `OpenAPI contract-first` · `Flyway` · `MapStruct` · `RabbitMQ` · `Resilience4j` · `SSE` · `PostgreSQL`

**Lenguajes**
`Java` · `Python` · `Bash` · `TypeScript`

**Sistemas y red**
`Linux (Arch, Debian, Kali, RHEL)` · `Windows Server` · `TCP/IP` · `DNS` · `DHCP` · `VLAN` · `Switching`

---

### Proyectos

**TARTIS Recon-AI — plataforma de gestión de parking** · *rol DevOps en un equipo de 15*
Multirepo de 5 microservicios Spring Boot con arquitectura hexagonal estricta y contrato OpenAPI primero. Mi parte es la plataforma: Kong como gateway y Keycloak como proveedor de identidad, RabbitMQ para la mensajería asíncrona, pipelines de GitHub Actions con gate de cobertura al 90% y análisis SonarCloud, branch protection uniforme en los 7 repos, y el stack completo levantándose tanto en Docker Compose como en Kubernetes con manifiestos Kustomize. Tests de contrato con Newman ejecutándose en CI.

**Homelab SOC** · *TFG de ASIR*
Stack de detección y respuesta sobre Proxmox: Wazuh como XDR, TheHive para gestión de casos, Cortex para análisis automatizado de observables, MISP como fuente de inteligencia y Shuffle para orquestar los playbooks. El objetivo es que una alerta llegue a caso enriquecido sin intervención manual.

**Infraestructura WordPress en AWS** · *[1dd0Rv/SREI](https://github.com/1dd0Rv/SREI/tree/wdpss_aws)*
VPC repartida en dos zonas de disponibilidad con subredes públicas y privadas: la base de datos queda aislada en la privada, sin ruta desde internet. EC2 Debian con LAMP y security groups por servicio, RDS MySQL como motor gestionado, y EFS montado por NFS para que `wp-content` sea compartido y la capa web pueda escalar horizontalmente. Documentado paso a paso.

---

```bash
$ ./contact_me.sh
> 1dd0rv@proton.me
> Abierto a hablar de plataforma, seguridad y automatización.
```
