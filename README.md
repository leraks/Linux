## Part 1
* ![part1](https://github.com/leraks/Linux/assets/67760549/094b363b-851c-429b-bb77-474e5bdafaec)
* Вывод версии Ubuntu
  
## Part 2
* ![image](https://github.com/leraks/Linux/assets/67760549/81a7bc46-49f9-4385-98f6-ab01744b2d34)
* ![image](https://github.com/leraks/Linux/assets/67760549/ec729475-7ffd-4f00-b645-e1de4a53123b)

## Part 3
* ![image](https://github.com/leraks/Linux/assets/67760549/eec2831c-e761-46b1-adef-4d5b7d2d86a8)
* lo – виртуальный интерфейс, присутствующий по умолчанию в любом Linux. Он используется для отладки сетевых программ и запуска серверных приложений на локальной машине. С этим интерфейсом всегда связан адрес 127.0.0.1. У него есть dns-имя – localhost.
*********
* ![image](https://github.com/leraks/Linux/assets/67760549/f4d8e5a8-67c2-4c54-803f-b64bacab00c8)
* DHCP - Cетевой протокол, позволяющий сетевым устройствам автоматически получать IP-адрес и другие параметры, необходимые для работы в сети TCP/IP.
*********
* ![image](https://github.com/leraks/Linux/assets/67760549/6d8268f3-0f63-4396-b8b4-501c21a4d79d)
*  внешний ip-адрес шлюза (ip)
* ![image](https://github.com/leraks/Linux/assets/67760549/5a07ac6a-9878-434b-a657-ad37ab24ad0e)
*  внутренний IP-адрес шлюза
*********
* ![image](https://github.com/leraks/Linux/assets/67760549/48388fab-0378-45ca-ba49-8295bb6fa5b7)
* статический ip, gw, dns
* ![image](https://github.com/leraks/Linux/assets/67760549/a0d2a335-b656-4b80-a280-b4892737ae5a)
* после перезагрузки данные остались
*********
* ![image](https://github.com/leraks/Linux/assets/67760549/15bb0450-13c6-462f-8212-a6589eddbeb2)
* ping google
* ![image](https://github.com/leraks/Linux/assets/67760549/7bae0f38-a559-4345-93ae-f00a70ec827f)
* ping yandex
* ![image](https://github.com/leraks/Linux/assets/67760549/c36b1b8d-f5f4-47d3-a874-4a4256a174d5)
* ping 1.1.1.1
  
## Part 4
![image](https://github.com/leraks/Linux/assets/67760549/3e6ba991-53bd-4a7b-b784-fe67d9a6d5f7)
*  Полное обновление системы

## Part 5
* ![image](https://github.com/leraks/Linux/assets/67760549/35357e86-a61e-4816-9434-64700edd4627)
* Изменение hostname ОС от имени пользователя, созданного в пункте Part 2 
* Команда sudo может использоваться для выполнения пользователем какой-либо команды, требующей права суперпользователя (root), то есть получение прав root для выполнения какой-либо команды на время её выполнения. Перед выполнением команды sudo запрашивает пароль пользователя

## Part 6
![image](https://github.com/leraks/Linux/assets/67760549/103371db-00a2-4d4c-ad98-987e4f11f0a9)
* Настроенное время в виртуальной среде

## Part 7
* ![image](https://github.com/leraks/Linux/assets/67760549/28b396f5-38f2-4f6c-8236-90bef5c75160)
  + vim ( esc + !wq )
* ![image](https://github.com/leraks/Linux/assets/67760549/e748d28a-bed1-4e27-a6db-871966459817)
  + nano ( ctrl + W AND ctrl + X)
* ![image](https://github.com/leraks/Linux/assets/67760549/52759887-fbba-4fda-abf6-8763edb86070)
  + joe ( ctrl K + B AND ctrl K + Q)
**********
* vim ( esc + q! )
* nano (ctrl + X В меню выбираем No)
* joe (ctrl K + Q В меню выбираем n)
**********
* ![image](https://github.com/leraks/Linux/assets/67760549/7d9a49a4-d952-431b-a744-3ca61726b3a4)
  + Поиск слова (vim)
* ![image](https://github.com/leraks/Linux/assets/67760549/81c0b022-4c93-4ad4-ba8e-c25e1a71a70d)
  + Замена слова (vim)
* ![image](https://github.com/leraks/Linux/assets/67760549/e45a85bf-5bf5-4700-8cca-17148a191430)
  + Поиск слова (nano)
* ![image](https://github.com/leraks/Linux/assets/67760549/1311465f-bdf0-4484-877d-de584f080658)
  + Замена слова (nano)
* ![image](https://github.com/leraks/Linux/assets/67760549/a2c0d1f9-65bc-4aed-ad78-1dd823074362)
  + Поиск слова (joe) ctrl G (Выбрать I)
* ![image](https://github.com/leraks/Linux/assets/67760549/1bec528e-f921-4377-8cf3-ca82459f4a76)
  + Замена слова  (joe) ctrl G (Выбрать R)

## Part 8
* Устоновка
  + sudo apt install openssh-server -y
  + # sudo systemctl enable ssh
* Настройка на 2022 порт
  + sudo cp /etc/ssh/sshd_config /etc/ssh/sshd_config.factory-defaults
  + sudo vi /etc/ssh/sshd_config
  + sudo systemctl restart ssh
* ![image](https://github.com/leraks/Linux/assets/67760549/486b04be-e06e-438c-807c-f9bbf958fd66)
* Наличие процесса sshd
  + Команда ps выводит список текущих процессов на вашем сервере в виде таблицы, с которой можно удобно работать: сортировать, изменять количество колонок и прочие.
* ![image](https://github.com/leraks/Linux/assets/67760549/629b15d1-6425-4613-bfda-9e2a0d6717bc)
  + Перечислить все порты: netstat -a
  + Перечислить все TCP порты: netstat -at
  + Команда покажет IP-адрес вместо хоста, номер порта вместо имени порта, UID вместо имени пользователя: netstat -an
  + Отображение активных сетевых подключений. Параметр -a отображает все активные сетевые подключения, параметр -ta отображает только информацию о TCP-соединениях, а параметр -tu отображает только информацию о UDP-трафике. Если опустить опцию -n, вместо IP-адресов будут печататься имена хостов.
  + В столбце Proto указан протокол, по которому ведется работа с портом.
  + В столбце Recv-Q приведено число пакетов, принятых ядром, но еще не прочитанных демоном, прослушивающим данный порт.
  + В столбце Send-Q отображается число пакетов, для которых ожидается подтверждение от удаленного узла.
  + В столбце Local Address показаны IP-адрес локального узала и логическое имя порта.
  + В поле Foreign Address отображаются IP-адрес удаленного узла и порт, с которым установлено соединение.
  + Столбец State применим только к TCP-соединениям и сообщает о состоянии соединения: CLOSING, CLOSED, CLOSE_WAIT, ESTABLISHED, FIN_WAIT1, FIN_WAIT2, LAST_ACK, LISTEN,SYN_SENT,SYN_RECV,TIME_WAIT.

## Part 9
* ![image](https://github.com/leraks/Linux/assets/67760549/009db630-a17a-49aa-99f4-50f5c019cd68)
  + uptime = 00:50:23
  + количество авторизованных пользователей =  ilua
  + общую загрузку системы = 0.0% бывает резкий
  + общее количество процессов = 103
  + загрузку cpu = 0.0%
  + загрузку памяти = 1971
  + pid процесса занимающего больше всего памяти = 1201
  + pid процесса, занимающего больше всего процессорного времени = 1
**********
* ![image](https://github.com/leraks/Linux/assets/67760549/f7983604-8b36-44c4-ba67-a212a788ba04)
  + отсортированному по PID
* ![image](https://github.com/leraks/Linux/assets/67760549/85d346ec-8de4-4466-8882-8757d84d141a)
  + отфильтрованному для процесса sshd
* ![image](https://github.com/leraks/Linux/assets/67760549/675f7442-6dce-48f1-a4f6-3bd0c7744c0e)
  + с процессом syslog, найденным, используя поискю
* ![image](https://github.com/leraks/Linux/assets/67760549/3ab32c0a-3637-4545-b301-cdcb4a2834bd)
  + с добавленным выводом hostname, clock и uptime

## Part 10
* ![image](https://github.com/leraks/Linux/assets/67760549/36419021-96d3-440f-9c2f-dcddcfc303a2)
  + Име VBOX HARDDISK
  + Размер 8gb
  + количество секторов 8589934592
  + 0 (не доконца понял но в команду free прописанно все по 0)

## Part 11
* ![image](https://github.com/leraks/Linux/assets/67760549/f872baa3-e641-4a61-8dfb-ba359a7dc9ca)
  + размер раздела = 6352332 kl
  + размер занятого пространства = 2929080 kl
  + размер свободного пространства = 3079396 kl
  + процент использования = 49%
* ![image](https://github.com/leraks/Linux/assets/67760549/d9a5abd4-1f58-4302-959a-a4ecc7c8ae73)
  + размер раздела = 6.1G
  + размер занятого пространства = 2.8G
  + размер свободного пространства = 3.0G
  + процент использования = 49%
* ![image](https://github.com/leraks/Linux/assets/67760549/a1b10924-9508-451f-a90e-e34ab37e3940)
  + ext4 — журналируемая файловая система

##  Part 12
* ![image](https://github.com/leraks/Linux/assets/67760549/8b8aba8b-df76-41ca-9c5f-020fac81ef83)
  +  размер папок /home, /var, /var/log
* ![image](https://github.com/leraks/Linux/assets/67760549/c039e4d9-c2f4-40d9-9228-ff3c52c365f8)
  + размер папок /home, /var, /var/log
*********
* ![image](https://github.com/leraks/Linux/assets/67760549/6c58f10f-dfc6-452f-a83d-53b4a01e4e65)
  +  размер всего содержимого в /var/log
  
## Part 13
* ![image](https://github.com/leraks/Linux/assets/67760549/50c0c2a5-68f5-445b-b485-24b17dfd2d60)
  + размер папок /home/
* ![image](https://github.com/leraks/Linux/assets/67760549/6443d7f1-b699-4903-8406-037bd36f7982)
  + размер папок /var/
* ![image](https://github.com/leraks/Linux/assets/67760549/b925b012-e4f5-402c-aa51-39c67b75712a)
  + размер папок /var/
  
## Part 14
* ![image](https://github.com/leraks/Linux/assets/67760549/eace90fc-dafd-4d32-83e2-20be68e68c37)
  + /var/log/dmesg просмотр
* ![image](https://github.com/leraks/Linux/assets/67760549/1314bc3d-f05c-4d53-b577-2ccfb2c7b5df)
  + /var/log/syslog просмотр
* ![image](https://github.com/leraks/Linux/assets/67760549/0018fa70-9789-4397-a648-dd7e32a2e435)
  + /var/log/auth.log
* ![image](https://github.com/leraks/Linux/assets/67760549/5d69b477-d0f7-44c1-a03b-58204a75f8f4)
  + Перезапустить службу SSHd
## Part 15
* ![image](https://github.com/leraks/Linux/assets/67760549/417ab9c3-7fc2-4945-8316-45e53f2a583e)
  + запуск команды uptime через каждые 2 минуты
* ![image](https://github.com/leraks/Linux/assets/67760549/4b2f0971-6284-48de-bc08-bba5a471f0b5)
  + список текущих заданий для CRON
* ![image](https://github.com/leraks/Linux/assets/67760549/5ce23e9e-7947-41fe-aa9f-05b32ee998bb)
  + Найти в системных журналах
* ![image](https://github.com/leraks/Linux/assets/67760549/16b4bbfa-dc49-47b7-b396-7c5b01230b53)
  +  списком текущих заданий для CRON после удаления









