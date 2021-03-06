# Отчет о лабораторной работе №1

## Цель

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину,
настройки минимально необходимых для дальнейшей работы сервисов.

## Ход работы

- Запустили терминал и перешли в каталог /var/tmp `cd var/tmp/`
- Создали каталог с именем пользователя `mkdir calixteGiordanny`
- Запустили виртуальную машину, введя в командной строке `Virtualbox &`
- Проверили в свойствах месторасположение каталога для виртуальной машины ![](https://github.com/calixteGiordanny/Lab_01/blob/main/report/img/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-04-29%2012-02-05.png "Рис. 1.1")
- Создали виртуальную машину
- Указали имя виртуальной машины
- Указали объем оперативной памяти виртуальной машины - 1024 МБ ![](https://github.com/calixteGiordanny/Lab_01/blob/main/report/img/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-04-29%2012-03-26.png)
- Задали конфигурацию и размер жесткого диска(40 ГБ) ![](https://github.com/calixteGiordanny/Lab_01/blob/main/report/img/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-04-29%2012-04-22.png)
  ![](https://github.com/calixteGiordanny/Lab_01/blob/main/report/img/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-04-29%2012-04-31.png)
  ![](https://github.com/calixteGiordanny/Lab_01/blob/main/report/img/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-04-29%2012-04-46.png)
- Добавили новый привод оптических дисков и выбрали образ afs/dk.sci.pfu.edu.ru/common/files/iso/CentOS-7-x86_64-DVD.iso
- Запустили виртуальную машину и перешли к настройкам операционной системы
- В разделе выбора программ указали в качестве базового окружения "Сервер с GUI",а в ка-честве дополнения — "Средств разработки"
- Отключили KDUMP ![](https://github.com/calixteGiordanny/Lab_01/blob/main/report/img/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-04-29%2012-23-07.png)
- Место установки ОС оставили без изменений ![](https://github.com/calixteGiordanny/Lab_01/blob/main/report/img/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-04-29%2012-25-29.png)
- Включили сетевое соединение и в качестве имени узла указали calixteGiordanny.localdomain ![](https://github.com/calixteGiordanny/Lab_01/blob/main/report/img/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-04-29%2012-25-17.png)
- Установили пароль для root с правами администратора ![](https://github.com/calixteGiordanny/Lab_01/blob/main/report/img/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA%20%D1%8D%D0%BA%D1%80%D0%B0%D0%BD%D0%B0%20%D0%BE%D1%82%202021-04-29%2012-28-08.png)
- После завершения установки корректно перезапустили систему и приняли лицензию
- Вошли в ОС под заданной при установке учетной записью и подключили образ диска дополненной гостевой ОС
- После загрузки дополнений нажали `Return` и `Enter` и перезагрузили систему\

## Контрольные вопросы

1. Учетная запись зхранит Системное Имя, Индетификатор пользователя, Индетификатор Группы, Домашний каталог
2. `cd ` для перемещения по файловой системе
   `--help` - для справки по команде, например ` cd --help`
   `ls` - для изучения содержимого файла
   `du` - для определения объема каталога
   `mkdir\rm` - для создания\удаления катлогов
   `chmod` - для задания прав на файл
   `history` - для просмотра истории команд
   3.Файловая система - порядок, определяющий способ организации, хранения и именования данных на носителях информации в компьютерах.
3. Чтобы посмотреть какие файловые системы подмонтированы в ОС надо ввести `ls proc/mounts`
4. Чтобы убить процесс надо ввести `kill` и PID процесса.
