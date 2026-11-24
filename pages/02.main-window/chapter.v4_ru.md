---
title: 'Главное окно'
taxonomy:
    category: docs
child_type: docs
media_order: 'main-window.png'
---

<style>
    #chapter p {
        text-align: left;
    }
</style>

### Раздел 2

# Главное окно

Главное окно QLC+ состоит из трех основных частей:

1.  Строка меню, с кнопками выполнения глобальных функций.
2.  Активные панели, выбираемые с помощью соответствующих вкладок.
3.  Вкладки, позволяющие переключаться между различными панелями QLC+.

![](/main-window/main-window.png)

Большинство элементов управления в программе снабжены всплывающими подсказками, которые появляются, если навести на них курсор мыши и задержать его на некоторое время.


### Строка меню (1)

Строка меню в верхней части окна рабочего пространства содержит следующие кнопки (слева направо):

* * *

![](../basics/filenew.png) Создать новый проект (CTRL+N)
![](../basics/fileopen.png) Открыть существующий проект (удерживайте кнопку нажатой, чтобы увидеть список недавно открывавшихся файлов) (CTRL+O)
![](../basics/filesave.png) Сохранить текущий проект (CTRL+S)
![](../basics/filesaveas.png) Сохранить текущий проект под новым именем

* * *

![](../basics/monitor.png)[DMX Monitor](dmx-monitor) (CTRL+M)  
![](../basics/diptool.png)[DMX Address tool](dmx-address-tool)  
![](../basics/audioinput.png)[Audio triggers](/virtual-console/audio-triggers)  

* * *

![](../basics/fullscreen.png) Переключить в полноэкранный режим (CTRL+F11)
![](../basics/help.png) Просмотреть документацию (Shift+F1)
![](../basics/qlcplus.svg?resize=32,32) Информация о QLC+

* * *

![](../basics/add_dump.png)[DMX Dump](dmx-dump): выгрузить и сохранить текущие значения DMX (CTRL+D)
![](../basics/liveedit.png)[Live Edit](live-edit): позволяет изменять функции, когда QLC+ находится в режиме управления (Operate Mode)
![](../basics/liveedit_vc.png) Live Edit для Виртуальной консоли (Virtual Console): позволяет изменять виртуальную консоль, когда QLC+ находится в режиме управления (Operate Mode). Для переключения обратно нажмите ещё раз.
![](../basics/panic.png) Остановить все функции (CTRL+Shift+ESC)
![](../basics/blackout.png) Включить/выключить режим `Блэкаут` (полное затемнение)
![](../basics/operate.png) Переключение между режимом проектирования (Design Mode) и режимом управления (Operate Mode) (CTRL+F12)


### Активная панель (2)

Здесь происходит всё основное действие. То, какая панель является активной, зависит от того, какая вкладка выбрана в данный момент.


### Вкладки панелей (3)

В нижней части главного окна расположены значки, предназначенные для переключения между различными рабочими средами (контекстами) QLC+.
Двойной щелчок по вкладке позволяет **отделить соответствующую рабочую среду в отдельное окно**. Чтобы вернуть её обратно в главное окно, достаточно просто закрыть это отдельное окно.
Рабочие среды QLC+ представлены в следующем порядке (слева направо):

![](../basics/fixture.png) Перейти к [Менеджеру приборов (Fixture Manager)](/fixture-manager)
![](../basics/function.png) Перейти к [Менеджеру функций (Function Manager)](/function-manager)
![](../basics/show.png) Перейти к [Менеджеру шоу (Show Manager)](/show-manager)
![](../basics/virtualconsole.png) Перейти к [Виртуальной консоли (Virtual Console)](/virtual-console)
![](../basics/slidermatrix.png) Перейти к [Простой панели управления (Simple Desk)](/simple-desk)
![](../basics/input_output.png) Перейти к настройкам [Входов/Выходов (Input/Output)](/input-output)
