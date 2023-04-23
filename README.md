# 5.5_Docker_Swarm_Aleksandr_Molokov

Задание 1

В чём отличие режимов работы сервисов в Docker Swarm кластере: replication и global?

# Ответ: Отличие в том, что в режиме global метрики передаются всем хостам. В режиме replication метрики передаются только тем хостам, у которых он указан.

Какой алгоритм выбора лидера используется в Docker Swarm кластере?

# Ответ: В Docker Swarm кластере используется так называемый алгоритм поддержания распределенного консенсуса — Raft. Выбор лидера происходит следующим образом: если ноды-фолловеры не слышат лидера, они переходят в статус кандидата, кандидат на лидера отправляет остальным нодам запрос на голосование и, большинством голосов, выбирается лидером.

Что такое Overlay Network?

# Ответ: Overlay network или наложенная сеть или оверлей — виртуальная сеть туннелей, работающая поверх физической.
L3-фабрика или IP-фабрика — потрясающее изобретение человечества, позволяющее к собеседованиям не повторять STP и не учить TRILL. Концепция, в которой вся сеть вплоть до уровня доступа исключительно L3, без VLAN и соответственно огромных растянутых широковещательных доменов.


Задание 2
# Ответ
ВМ yandexCloud

![yandex vm](https://user-images.githubusercontent.com/109212419/233840856-e08b8bd5-31b1-4aab-8525-41f20f94bd87.jpg)

Инициализация manager

![initialase manager1 like manage node](https://user-images.githubusercontent.com/109212419/233840874-d993c10d-5cf5-4d14-95b7-61cc69a338a0.jpg)

Присоединение workers

![join workers on claster](https://user-images.githubusercontent.com/109212419/233840891-33852f1c-6553-436a-89d5-bd8ebd645c7f.jpg)

![tack 2 docker node ls](https://user-images.githubusercontent.com/109212419/233840451-74519d1f-b7dc-4279-b853-bb0e0e8b075a.jpg)

Задание 3
# Ответ
![docker service ls](https://user-images.githubusercontent.com/109212419/233840465-f97b522d-f544-4953-b650-6fdfca081113.jpg)

![Docker-compose.yml](https://github.com/ALEMOLOKOV/5.5_Docker_Swarm_Aleksandr_Molokov/blob/e9ed3c38aaea3838906bf35b3499ca20c5a71785/docker-compose.yml)

# Проверка
Сервис голосования

![голосование](https://user-images.githubusercontent.com/109212419/233840626-192ca332-d4f7-4466-a1c2-4d396d50b2f3.jpg)

Результаты

![результат голосования](https://user-images.githubusercontent.com/109212419/233840640-e01265a9-0a40-4139-93ed-a63050ab0c43.jpg)


