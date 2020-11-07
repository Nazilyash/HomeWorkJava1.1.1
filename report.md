# **Отчёт о тестировании `OpenJDK11` и `KeyValidator`**

## **Краткое описание**

<07/11/2020> - <07/11/2020> было проведено:
- тестирование установки OpenJDK11 (работа инструкции по установке OpenJDK11 под ОС, процесс установки OpenJDK11);
- тестирования OpenJDK11 (в процессе работы с KeyValidator):  конфигурационное (совместимость с ОС) и функциональное  (функции работы с KeyValidator); 
- тестирования  KeyValidator: функциональное (запуск, работа согласно руководству использования) и конфигурационное (совместимость с OpenJDK11).

*На тестирование затрачено:* <2ч>

*В результате тестирования выявлены следующие дефекты:*
1. [баг 1](https://github.com/Nazilyash/HomeWorkJava1.1.1/issues/1) После установки OpenJDK 11 при выполнении в терминале git команды "java -version" выходит сообщение об ошибке;
1. [баг 2](https://github.com/Nazilyash/HomeWorkJava1.1.1/issues/2) KeyValidator в терминале git при проверке ключей неверно оценивает их валидность.

## **Описание процесса тестирования**

**В процессе тестирования использовались следующие артефакты:**

- отчет о тестировании;   
- баг-репорты.


**В качестве тестовых данных использовались данные:**

1. [Инструкция по установке OpenJDK11](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md) (для Windows);

1. [Руководство использования KeyValidator](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md).


**Тестирование производилось в следующем окружении:*

- ОС Microsoft Windows 7 Домашняя базовая Версия 6.1.7601 Service Pack 1 Сборка 7601, разрядность: 64-битная;

- openjdk version "11.0.9" 2020-10-20, OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.9+11),
OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.9+11, mixed mode);

- Google Chrome Версия 86.0.4240.183 (Официальная сборка), (64 бит);

- Visual Studio Code версия 1.50.1.