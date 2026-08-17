# OpenShift Labs — Índice de proyectos

Repositorio índice: un solo lugar para ver de qué trata cada demo/proyecto de OpenShift sin tener que entrar carpeta por carpeta. Cada fila enlaza al repo real, que tiene su propio README con el detalle de despliegue.

| Proyecto | Descripción | Repo |
|----------|-------------|------|
| **Instalacion-OpenShift-4** | Guía paso a paso de instalación de OpenShift 4 Bare Metal, UPI (User Provisioned Infrastructure), para ambientes de demo/desarrollo. | [github.com/trixlan/Instalacion-OpenShift-4](https://github.com/trixlan/Instalacion-OpenShift-4) |
| **podman-openshift** | API REST de catálogo de productos (Quarkus + PostgreSQL). Desarrollo local con Podman y despliegue en OpenShift vía `oc` CLI. | [github.com/trixlan/podman-openshift](https://github.com/trixlan/podman-openshift) |
| **balanceador-openshift** | Demo de balanceo de carga entre réplicas de un Service. Dashboard web que muestra en vivo qué pod y nodo atendió cada petición. Despliegue manual con `oc` o fast track con Ansible. | [github.com/trixlan/balanceador-openshift](https://github.com/trixlan/balanceador-openshift) |
| **AB-openshift** | Traffic splitting con OpenShift Routes (`alternateBackends`, split 90/10 configurable). Incluye dashboard web con la distribución v1/v2 en vivo y despliegue fast track con Ansible. | [github.com/trixlan/AB-OpenShift](https://github.com/trixlan/AB-OpenShift) |
| **ocp-custom-metrics-keda** | Autoscaling de una aplicación con KEDA a partir de métricas de OpenShift Monitoring (Prometheus/Thanos), usando el Custom Metrics Autoscaler operator. | [github.com/trixlan/OCP-Custom-Metrics-KEDA](https://github.com/trixlan/OCP-Custom-Metrics-KEDA) |
| **RBAC** | Demo de RBAC en OpenShift: 4 ServiceAccounts con distintos niveles de permisos (`view`, `edit`, `admin`, un `Role` custom) en el mismo namespace, con script que valida con `oc auth can-i` qué puede hacer cada uno. | [github.com/trixlan/RBAC](https://github.com/trixlan/RBAC) |
| **Tekton** | Pipeline de OpenShift Pipelines (Tekton) que automatiza CI/CD de una app Node.js: clone → build → deploy → verify, con smoke test contra un endpoint `/info` y dashboard en vivo del despliegue. | [github.com/trixlan/Tekton](https://github.com/trixlan/Tekton) |

## Cómo agregar un proyecto nuevo

1. Agrega una fila a la tabla de arriba: nombre, descripción de 1-2 líneas y link al repo en GitHub.
2. Verifica que el repo del proyecto tenga su propio README con instrucciones de despliegue (paso a paso + fast track si aplica).
3. Haz commit y push aquí — no se necesita tocar nada en los repos individuales.
