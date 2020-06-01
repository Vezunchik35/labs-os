 -ФИО: Махсудов Далер Улмасжонович
Группа: ББСО-04-18
Часть №1 Начало : установка ос и настройка RAID и LVM. (screenshots -> part1)
Создаем виртуальную машину с характеристиками : 1gb ram, 1 cpu, 2 hdd - (sdd1, ssd2), SATA контройлер настроен на 4 порта.

## Часть №1 Начало : установка ос и настройка RAID и LVM. (screenshots -> part1)
- Создаем виртуальную машину с характеристиками : 1gb ram, 1 cpu, 2 hdd - (sdd1, ssd2), SATA контройлер настроен на 4 порта.

- Скриншот 1.1 - показывает нам настройку разметки дисков.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.1.png)
- Скриншот 1.2 - первое разделение дисков.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.2.png)
- Скриншот 1.3 - указание места для RAID.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.3.png)
- Скриншот 1.4 - настроиваем RAID.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.4.png)
- Скриншот 1.5 - начало установки и настройки LVM.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.5.png)
- Скриншот 1.6 - середина настройки LVM.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.6.png)
- Скриншот 1.7 - конечная настройка и установка LVM.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.7.png)
- Скриншот 1.8 - результат настройки и установки LVM.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.8.png)
- Скриншот 1.9 - установка GRUB на первый диск (sda).
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.9.png)
- Скриншот 1.10 - первая информация о дисках.

![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.10.png)
- Скриншот 1.11 - первая информация о RAID.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.11.png)
- Скриншот 1.12 - первая информация о pvs, vgs, lvs.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part1/1.12.png)

# Часть №2 По заданию отключается один SSD,по заданию мы заменяем его и с помощью LVM сохраняем все данные и копируем на новый диск. (screenshots -> part2)

- Скриншот 2.1 - реакция ос на удаление ssd1.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part2/2.1.png)
- Скриншот 2.2 - виртуальная машина работает.

![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part2/2.2.png)
- Скриншот 2.3 - проверка статуса RAID после удаление sdd1.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part2/2.3.png)
- Скриншот 2.4 - реакция виртуальной машины на добавление ssd3.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part2/2.4.png)
- Скриншот 2.5 - добавление в RAID ssd3.

![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part2/2.5.png)
- Скриншот 2.6 - результат в mdstat.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part2/2.6.png)
- Скриншот 2.7 - результат задания №2.

![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part2/2.7.png)

# Часть №3 В этой части по заданию отключается еще один SSD, мы заменяем его на новый sdd на 7 gb и добавляем 2 новых HDD.
С помощью LVM и RAID спасаем данные и включаем новый SSD в VG. (screenshots -> part3)
- Скриншот 3.1 - информация о дисках после удаления ssd2.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.1.png)
- Скриншот 3.2 - информация в mdstat после удаления ssd2.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.2.png)
- Скриншот 3.3 - информация после добавления ssd4.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.3.png)
- Скриншот 3.4 - информация после копирования файлов в таблицу на ssd4.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.4.png)
- Скриншот 3.5 - информация после монтирования boot на ssd4.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.5.png)
- Скриншот 3.6 - информация после создания нового RAID массива.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.6.png)
- Скриншот 3.7 - изменение pvs до и после создания нового zip тома.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.7.png)
- Скриншот 3.8 - информация о дисках после создания zip тома.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.8.png)
- Скриншот 3.9 - var, root, var находятся на md0.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.9.png)
- Скриншот 3.10 - результаты после перемещения LV.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.10.png)
- Скриншот 3.11 - информация о дисках только после добавления всех новых.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.11.png)
- Скриншот 3.12 - информация о дисках после копирования таблицы файлов и sda1.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.12.png)
- Скриншот 3.13 - информация после добавления ssd5 в RAID и увеличения размеров на общих дисках.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.13.png)
- Скриншот 3.14 - размер  sda(e)2=md127.

![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.14.png)
- Скриншот 3.15 - размер VG увеличился.

![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.15.png)
- Скриншот 3.16 - информация об увеличении размеров root и var.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.16.png)
- Скриншот 3.17 - конечный результат работы с ssd.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.17.png)
- Скриншот 3.18 - информация о дисках после создания логического тома.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.18.png)
- Скриншот 3.19 - информация о дисках после форматирования разделов.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.19.png)
- Скриншот 3.20 - информация о дисках после переформатирования var-логов.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.20.png)
- Скриншот 3.21 - изменение файла fstab.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.21.png)
- Скриншот 3.22 - последняя проверка pvs, lvs, vgs.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.22.png)
- Скриншот 3.23 - послежняя проверка и информация о дисках.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.23.png)
- Скриншот 3.24 - последняя информация о RAID.
![Image alt](https://github.com/batasov/oslabs/raw/master/lab2/screenshots/part3/3.24.png)
