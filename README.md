# Домашнее задание  "Репликация и масштабирование. Часть 1" - Храмов Александр

---

### Задание 1.

На лекции рассматривались режимы репликации master-slave, master-master, опишите их различия.
master-slave есть основной сервер, остальные копии (slave) которые считывают обновления с мастера и вносят себе изменения. 
Это полезно если нужно распараллелить нагрузку при этом приложения работают на чтения с slave (много), а запись только в master (мало)

maste-master все тоже самое только каждый узел становится еще мастером для последующего. Такой конфиг удачен для зональных серверов которые обслуживают 
определенную локацию и в каждом такой зоне работает master. При DRP (Disaster Recovery Plan)  будет переключен на master других зон. 

*Ответить в свободной форме.*

---

### Задание 2.

Выполните конфигурацию Master-Slave репликации (примером можно пользоваться из лекции).

*Приложите скриншоты конфигурации, выполнения работы (состояния и режимы работы серверов).*


![alt text](https://github.com/vasev85/sql_replication1/blob/main/screens/ex2-1.png?raw=true)
![alt text](https://github.com/vasev85/sql_replication1/blob/main/screens/ex2-2.png?raw=true)
![alt text](https://github.com/vasev85/sql_replication1/blob/main/screens/ex2-3.png?raw=true)


---

## Дополнительные задания (со звездочкой*)

Эти задания дополнительные (не обязательные к выполнению) и никак не повлияют на получение вами зачета по этому домашнему заданию. Вы можете их выполнить, если хотите глубже и/или шире разобраться в материале.

---

### Задание 3*. 

Выполните конфигурацию Master-Master репликации. Произведите проверку.

*Приложите скриншоты конфигурации, выполнения работы (состояния и режимы работы серверов).*

![alt text](https://github.com/vasev85/sql_replication1/blob/main/screens/ex3-1.png?raw=true)
![alt text](https://github.com/vasev85/sql_replication1/blob/main/screens/ex3-2.png?raw=true)
![alt text](https://github.com/vasev85/sql_replication1/blob/main/screens/ex3-3.png?raw=true)