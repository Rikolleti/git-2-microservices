# Домашнее задание к занятию «Микросервисы: масштабирование»

## Задача 1: Кластеризация

Контейнеры: Docker-образы в Yandex Container Registry (или Docker Hub).

Платформа оркестрации: Kubernetes.

Сервис-дискавери и маршрутизация: встроенный kube-dns + Services (ClusterIP) и Ingress-контроллер (NGINX).

Горизонтальное масштабирование: Kubernetes HPA (Horizontal Pod Autoscaler).

Авто-масштабирование кластера: Cluster Autoscaler Yandex Cloud.

Разделение внешних/внутренних ресурсов: Service types (ClusterIP — внутрь, LoadBalancer/Ingress(API) — наружу), а также настройки сетевой политики для повышения безопасности.

Конфиги и секреты: ConfigMap и Secret (env-переменные).

Деплой: - GitLab CI

Мониторинг: Prometheus + Grafana, ELK.
