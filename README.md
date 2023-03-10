# Домашнее задание к занятию "`10.3 Pacemaker`" - `Никулин Михаил Сергеевич`



---

### Задание 1

`Pacemaker - это наиболее широко используемый диспетчер ресурсов кластера с открытым исходным кодом в среде Linux. 
Pacemaker использует функции управления сообщениями и элементами кластера, предоставляемые инфраструктурой 
кластера (Corosync или Heartbeat), для обнаружения сбоев на уровне узлов и ресурсов и восстановления ресурсов, 
тем самым обеспечивая максимальную надежность и высокую доступность кластерных сервисов.` 

`Основные функции:`

- `позволяет находить и устранять сбои на уровне нод и служб;`
- `не зависит от подсистемы хранения: нет требования к общему накопителю;`
- `не зависит от типов ресурсов: все, что можно прописать в скрипты, можно кластеризовать;`
- `поддерживает STONITH (Shoot-The-Other-Node-In-The-Head), то есть умершая нода изолируется и запросы к ней не поступают, пока нода не отправит сообщение о том, что она снова в рабочем состоянии;`
- `поддерживает кворумные и ресурсозависимые кластеры любого размера;`
- `поддерживает практически любую избыточную конфигурацию;`
- `может автоматически реплицировать конфиг на все узлы кластера — не придется править все вручную;`
- `можно задать порядок запуска ресурсов, а также их совместимость на одном узле;`
- `поддерживает расширенные типы ресурсов: клоны (когда ресурс запущен на множестве узлов) и дополнительные состояния (master/slave и подобное) — актуально для СУБД (MySQL, MariaDB, PostgreSQL, Oracle);`
- `имеет единую кластерную оболочку CRM с поддержкой скриптов.`


---

### Задание 2

`Corosync — это программный продукт, позволяющий реализовать кластер
серверов. Его основное назначение — знать и передавать
состояние всех участников кластера.`


`В основе работы заложены следующие функции:`

- `отслеживание состояния приложений;`
- `оповещение приложений о смене активной ноды кластера;`
- `отправка одинаковых сообщений процессам на всех узлах
кластера;`
- `предоставление доступа к базе данных с конфигурацией и
статистикой, а также отправка уведомлений о ее изменениях.`


---

### Задание 3

![pcs_status.png](img%2Fpcs_status.png)
![cluster_web.png](img%2Fcluster_web.png)
![corosync_conf.png](img%2Fcorosync_conf.png)
![pcs_backup.png](img%2Fpcs_backup.png)

---
## Дополнительные задания (со звездочкой*)


### Задание 4*

![drbdadm_status.png](img%2Fdrbdadm_status.png)
![mysql.png](img%2Fmysql.png)
![www.png](img%2Fwww.png)
