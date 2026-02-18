# -Домашнее задание к занятию «Запуск приложений в K8S»-

## Задание 1. 
Создать Deployment и обеспечить доступ к репликам приложения из другого Pod
Создать Deployment приложения, состоящего из двух контейнеров — nginx и multitool. Решить возникшую ошибку.
После запуска увеличить количество реплик работающего приложения до 2.
Продемонстрировать количество подов до и после масштабирования.
Создать Service, который обеспечит доступ до реплик приложений из п.1.
Создать отдельный Pod с приложением multitool и убедиться с помощью curl, что из пода есть доступ до приложений из п.1.

### Ответ
<img width="499" height="136" alt="2_1" src="https://github.com/user-attachments/assets/bd1e0e3c-379e-458c-83cb-2398e27e8c53" />
<img width="494" height="104" alt="2_2" src="https://github.com/user-attachments/assets/e2248677-79ea-42cc-a41b-715a11c9af52" />
<img width="689" height="272" alt="2_3" src="https://github.com/user-attachments/assets/4c29642c-aa96-4501-a622-f80e9e515957" />
[deployment](https://github.com/Nano-prototip/-K8S/blob/main/deployment.yml).
[service](https://github.com/Nano-prototip/-K8S/blob/main/service.yml).
[pod](https://github.com/Nano-prototip/-K8S/blob/main/pod.yml).

## Задание 2. 
Создать Deployment и обеспечить старт основного контейнера при выполнении условий
Создать Deployment приложения nginx и обеспечить старт контейнера только после того, как будет запущен сервис этого приложения.
Убедиться, что nginx не стартует. В качестве Init-контейнера взять busybox.
Создать и запустить Service. Убедиться, что Init запустился.
Продемонстрировать состояние пода до и после запуска сервиса.

### Ответ
<img width="684" height="545" alt="2_4" src="https://github.com/user-attachments/assets/ea53b11e-5d1a-4b3f-91a8-56b90510d871" />
[deployment](https://github.com/Nano-prototip/-K8S/blob/main/deployment2.yml).
