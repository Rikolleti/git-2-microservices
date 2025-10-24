# Домашнее задание к занятию «Микросервисы: масштабирование»

## Задача 1: Кластеризация

Контейнеры: Docker-образы в Yandex Container Registry (или Docker Hub).

Платформа оркестрации: Kubernetes (YC Managed Kubernetes либо minikube/Kind для локальных тестов).

Сервис-дискавери и маршрутизация: встроенный kube-dns + Services (ClusterIP/Headless) и Ingress-контроллер (NGINX/Traefik).

Горизонтальное масштабирование: HPA (Horizontal Pod Autoscaler).

Авто-масштабирование кластера: Cluster Autoscaler Yandex Cloud.

Разделение внешних/внутренних ресурсов: Service types (ClusterIP — внутрь, LoadBalancer/Ingress — наружу), Сетевые политики.

Конфиги и секреты: ConfigMap и Secret (env-переменные). Для безопасного хранения — External Secrets + Yandex Lockbox (KMS).

Деплой: - GitLab CI

Наблюдаемость (по минимуму): Prometheus + Grafana, ELK.
