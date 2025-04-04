# Домашнее задание к занятию «Система мониторинга Zabbix. Часть 2»

## Шкутов Иван Владимирович


#### В практике есть 4 основных и 5 дополнительных (со звездочкой) заданий. Основные задания нужно выполнять обязательно, со звездочкой - по желанию и его решение никак не повлияет на получение вами зачета по этому домашнему заданию, при этом вы сможете глубже и/или шире разобраться в материале.

Пожалуйста, присылайте на проверку все задачи сразу. Любые вопросы по решению задавайте в чате учебной группы.

#### <ins>Цели задания</ins>

1. Научитья создавать свои шаблоны в Zabbix, добавлять в Zabbix хосты и связывать шаблон с хостами

2. Научиться составлять кастомный дашборд

3. Научиться создавать UserParameter на Bash

4. Научиться создавать Python-скрип, добавляться в него UserParameter и прикреплять к шаблону

5. Научиться создавать Vagrant-скрипты для Zabbix Agent

#### <ins>Чеклист готовности к домашнему заданию</ins>

Просмотрите в личном кабинете занятие "Система мониторинга Zabbix. Часть 2"

#### <ins>Инструкция по выполнению домашнего задания</ins>

1. Сделайте fork репозитория c шаблоном решения к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/gitlab-hw или https://github.com/имя-вашего-репозитория/8-03-hw).

2. Выполните клонирование этого репозитория к себе на ПК с помощью команды git clone.

3. Выполните домашнее задание и заполните у себя локально этот файл README.md:

   - впишите вверху название занятия и ваши фамилию и имя;
   
   - в каждом задании добавьте решение в требуемом виде: текст/код/скриншоты/ссылка;
   
   - для корректного добавления скриншотов воспользуйтесь инструкцией «Как вставить скриншот в шаблон с решением»;
   
   - при оформлении используйте возможности языка разметки md. Коротко об этом можно посмотреть в инструкции по MarkDown.

4. После завершения работы над домашним заданием сделайте коммит (git commit -m "comment") и отправьте его на Github (git push origin).

5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.

6. Любые вопросы задавайте в чате учебной группы и/или в разделе «Вопросы по заданию» в личном кабинете.


## Задание 1
 Создайте свой шаблон, в котором будут элементы данных, мониторящие загрузку CPU и RAM хоста.

#### <ins>Процесс выполнения</ins>

1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции
   
3. В веб-интерфейсе Zabbix Servera в разделе Templates создайте новый шаблон
   
5. Создайте Item который будет собирать информацию об загрузке CPU в процентах
   
7. Создайте Item который будет собирать информацию об загрузке RAM в процентах
   
#### <ins>Требования к результату</ins>

 1. Прикрепите в файл README.md скриншот страницы шаблона с названием «Задание 1»


---

## Задание 2
 Добавьте в Zabbix два хоста и задайте им имена <фамилия и инициалы-1> и <фамилия и инициалы-2>. Например: ivanovii-1 и ivanovii-2.

#### <ins>Процесс выполнения</ins>

1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции

2. Установите Zabbix Agent на 2 виртмашины, одной из них может быть ваш Zabbix Server

3. Добавьте Zabbix Server в список разрешенных серверов ваших Zabbix Agentов

4. Добавьте Zabbix Agentов в раздел Configuration > Hosts вашего Zabbix Servera

5. Прикрепите за каждым хостом шаблон Linux by Zabbix Agent

6. Проверьте что в разделе Latest Data начали появляться данные с добавленных агентов
   
#### <ins>Требования к результату</ins>

 1. Результат данного задания сдавайте вместе с заданием 3

---

## Задание 3
 Привяжите созданный шаблон к двум хостам. Также привяжите к обоим хостам шаблон Linux by Zabbix Agent.

#### <ins>Процесс выполнения</ins>

1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции

2. Зайдите в настройки каждого хоста и в разделе Templates прикрепите к этому хосту ваш шаблон

3. Так же к каждому хосту привяжите шаблон Linux by Zabbix Agent

4. Проверьте что в раздел Latest Data начали поступать необходимые данные из вашего шаблона
   
#### <ins>Требования к результату</ins>

 1. Прикрепите в файл README.md скриншот страницы хостов, где будут видны привязки шаблонов с названиями «Задание 2-3». Хосты должны иметь зелёный статус подключения

---

## Задание 4
 Создайте свой кастомный дашборд.

#### <ins>Процесс выполнения</ins>

1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции

2. В разделе Dashboards создайте новый дашборд

3. Разместите на нём несколько графиков на ваше усмотрение
   
#### <ins>Требования к результату</ins>

 1. Прикрепите в файл README.md скриншот дашборда с названием «Задание 4»


---
