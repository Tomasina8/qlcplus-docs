---
название: 'Глоссарий и понятия'
дата: '19:56 17-11-2026'
---

Q Light Controller Plus (сокращённо QLC+) предназначен для управления осветительным оборудованием, используемым в различных видах деятельности, например, живые концерты, театры и т.д. Основная цель QLC+ заключается в том, чтобы превзойти коммерческие пульты управления светом без необходимости использования 500-страничного руководства благодаря интуитивно понятному и гибкому пользовательскому интерфейсу.

Эта страница содержит определения в алфавитном порядке, чтобы облегчить поиск по конкретной теме.

### ! [](../audio.svg) Аудио

Аудио [функция](#functions) - объект, представляющий аудиофайл, хранящийся на диске.  
QLC+ поддерживает самые распространённые аудиоформаты, такие как Wave, MP3, M4A, Ogg и Flac. Поддержка моно- и стереоканалов и несколько частот дискретизации, таких как 44,1 кГц, 48 кГц и т.д.  
Аудиофункции могут быть размещены в [Chaser](#chaser) или в [Show](#show) в нужное время с помощью панели [Show Manager](/show-manager).  
Как и большинство функций QLC+, аудио поддерживает время входа и выхода.  

### ! [](../blackout.svg) Blackout (Полное затемнение)

Blackout - это специальная функция QLC+, используемая для установки всех [HTP](#htp-highest-takes-precedence) каналов во всех Вселенных на ноль. Это приведет к полному погашению всех световых приборов. Каналы останутся на нуле, независимо от текущих функций или значений, назначенных им вручную (например, из [Simple Desk](/simple-desk). Когда Полное затемнение завершается, все каналы снова будут управляться функциями или их значением, заданным вручную. 

### Возможности (параметры канала)

Некоторые каналы в интеллектуальных приборах предоставляют множество функций или возможностей, таких как включение лампы при значении канала [240-255], настройка красного цвета на цветовом колесе при точном значении [15]] или просто управление яркостью с помощью значений [0-255]. Каждая из этих индивидуальных функций называется возможностью, и у каждой из них есть следующие свойства:

*   Минимальное значение: минимальное значение канала, предоставляющего возможность.
*   Максимальное значение: максимальное значение канала, предоставляющего возможность.
*   Имя: удобне оператору название
*   Преднастройка: предопределенная функция, позволяющая QLC+ точно распознавать, как обрабатывать и имитировать значение канала

### ! [](../chaser.svg) Chaser (Чейзер)

Chaser [function](#functions) формируется из нескольких сцен, которые выполняются последовательно, один за другим, когда функция chaser запускается. Следующая функция выполняется только после завершения предыдущей. Любое количество [функций](#functions) может быть добавлено в чейзер.

Направление функции Chaser может быть развернуто в обратную сторону, также сцены в пределах чейзера может быть случайным. Функция Chaser также может быть настроена на бесконечный цикл, бесконечный пинг-понг-цикл (направление реверсируется после каждого прохождения) или она может проходить только один раз, в одноразовом режиме, после чего завершается. Если функция настроена на бесконечный цикл, она должна быть остановлена вручную.

Каждый Chaser имеет свои параметры скорости:

*   **Появление:** Скорость появления шага
*   **Удержание:** Время удержания шага
*   **Затухание:** Скорость затухания шага
*   **Длительность:** Общая продолжительность функции

Копии функций chaser можно создать с помощью [Function Manager](/function-manager). Сцены внутри чейзера не дублируются при копировании чейзера. В новый чейзер копируются только порядок и направление.

### Click And Go (Нажмите и перейдите)

Click And Go - это технология, которая позволяет оператору быстро перейти к макросам и цветам визуально и всего за пару кликов. Это позволяет проводить более эффектные живые шоу и  свободу выбора желаемого результата.
На данный момент доступны три типа виджетов:

*   Одноцветный (применяется к: красным, зелёным, синим, синим, желтым, магутиновым, янтарным и белым каналам интенсивности)
*   RGB Color Picker. Позволяет выбрать значения для выбранных каналов RGB одним щелчком мыши
*   Выбор гобо/макросов. Доступ и отображение гобо/макроса, определенного в параметрах светового прибора.

Обзор со скриншотами доступен [здесь] (https://www.qlcplus.org/old/clickandgo.html)

### ! [](../collection.svg) Collection (Коллекция)

Функция Collection [function](#functions) соединяет несколько функций, которые выполняются одновременно при запуске collection. Любое количество функций может быть добавлено в коллекцию, но каждая функция может быть вставлена только один раз и коллекция не может быть прямым членом самой себя.

Коллекции не имеют параметров скорости. Скорость каждой функции участника устанавливается индивидуально с помощью собственных редакторов.

Копии функций коллекции могут быть созданы с помощью [Function Manager](/function-manager). Функции, содержащиеся в коллекции, не дублируются; копируется только список функций.

### DMX

[DMX](https://en.wikipedia.org/wiki/DMX512) - сокращение для Digital MultipleX. Этотр интерфейс определяет целый ряд свойств: протокол, электрические соединения и т.д. В случае светового программного обеспечения он определяет максимальное количество каналов (512) на вселенную и диапазон значений каждого канала (0-255).

QLC+ поддерживает неограниченное количество вселенных (изначально есть 4, но при необходимости можно добавить больше). Они не обязательно должны быть подключены к оборудованию DMX. Фактическая аппаратная абстракция (независимо от того, является ли она аналоговой (0-10 В), DMX или каким-либо другим методом) достигается через [output plugins](#input-output-plugins).

### ! [](../efx.svg) EFX

EFX [function](#functions) в основном используется для автоматизации движущихся огней (например, сканеров и движущихся головок), хотя он также может автоматизировать значения RGB или Dimmer недвижущихся огней. EFX может создавать сложные математические пути на плоскости Х-Y, которые преобразуются в значения DMX для поля и наклона устройства или каналов RGB или Dimmer.

### ! [](../fixture.svg) Fixtures (Световые приборы)

Каждый Прибор - по сути, одно устройство освещения. Это может быть, например, один прожектор, одна движущаяся голова, один сканер, один лазер и т.д. Однако для простоты отдельные PAR-прожекторы (и подобные им), которые обычно управляются по одному каналу, могут быть сгруппированы вместе, чтобы образовать одну световую установку.

С помощью редактора параметров прибора оператор может редактировать общие сведения о световом приборе, хранящиеся в файле описания прибора, и содержит следующие свойства для каждого из них:

*   Производитель (например, ClayPaky)
*   Модель (например, MAC250)
*   Тип (цветовой прожектор, сканер, вращающаяся голова, дым-машина, туман, вентилятор...)
*   Физические свойства (тип источника счета, угол луча, размеры...)
*   Каналы:
    *   Группа каналов (Яркость, Панорама, Наклон, Гобо, Цвет, Скорость и т.д.)
    *   Привязка 8-битных и 16-битных каналов для групп Панорама и Наклон
    *   Дополнительный основной цвет для каналов интенсивности (RGB/CMY)
    *   Диапазоны значений для функций канала (например, 0-5: лампа включена, 6-15: мерцание и т.д.).

Эти параметры приборов могут быть затем использованы для создания фактических приборов в приложении Q Light Controller Plus, которые будут иметь дополнительные свойства, определенные оператором:

*   Вселенная DMX
*   Адрес DMX
*   Имя

Можно создать несколько экземпляров прибора (например, у световго оператора есть несколько световых приборов MAC250). Каждый прибор может быть поименован, но назване не используется внутри QLC+ для идентификации отдельных экземпляров. То же самое относится к адресу DMX. Тем не менее, операторам рекомендуется называть свои устройства каким-либо внятным образом, чтобы через некоторое время не всмопинать где какой из них.

Обычные одноканальные световые приборы (например, одноцветные прожекторы) в режиме диммирования не требуют особых определений, ибо обычно они используются группами. Операторы могут создавать экземпляры этих общих приборов, просто определяя количество каналов для каждого из них.

### ! [](../group.svg) Fixture Group (Группа приборов)

Группа приборов - это условное название группы [артикулов](#артикулов). Часто для удобства они обозначаются фактическое физическое расположение этих приборов в реальном шоу. Это знание может быть использовано, например, в RGB Matrix для создания стены RGB-огней, которые могут действовать как отдельные пиксели в графическом узоре или текстовой прокрутке.

### Fixture Mode (Режим прибора)

Многие производители выпускают свои световые приборы таким образом, что они имеют несколько различных наборов каналов. Например, сканер может иметь два варианта конфигурации: один для только 8-битных каналов перемещения (1x pan, 1x tilt) и другой для 16-битных каналов перемещения (2x pan, 2x tilt). Вместо создания совершенно нового определения прибора для каждого варианта, они были объединены в рамках определений прибора QLC+ в понятие Режим. Другие программы управления светом иногда называют режимы «личностью».

### ![](../functions2.svg) Functions

The number of functions is practically unlimited. Functions are used to automate the setting of values to DMX channels. Each function type has its own way of automating lights.

The function types are:

*   [Scene](#scene)
*   [Chaser](#chaser)
*   [Sequence](#sequence)
*   [EFX](#efx)
*   [RGB Matrix](#rgb-matrix)
*   [Collection](#collection)
*   [Show](#show)
*   [Audio](#audio)
*   [Video](#video)

Each function can be named and, although the name is not used to uniquely identify individual functions, users are encouraged to name their functions in some systematic and concise way to help identify each of them. For your own comfort.

Each function has its own speed settings:

*   **Fade In:** The time used to fade HTP (in Scenes also LTP) channels to their target value
*   **Fade Out:** The time used to fade HTP/intensity channels back to zero
*   **Duration:** The duration of the current step (not applicable on Scenes)

### Grand Master

The Grand Master is used as the final master slider before values are written to the actual physical DMX hardware. Usually, the Grand Master affects only **Intensity** channels, but can also be changed to effect the values of **all** channels.

The Grand Master has also two **Value Modes** that control the way _how_ the Grand Master affects channel values:

*   Reduce: Affected channels' values are reduced by a percentage set with the Grand Master slider. For example, Grand Master at 50% will result in all affected channels being reduced to 50% of their **current** values.
*   Limit: Affected channels cannot get larger values than the value set with the Grand Master slider. For example, Grand Master at 127 will result in all the affected channels' maximum values being limited at exactly 127.

### Head

A head represents an individual light output device in a fixture. Usually, a single fixture contains exactly one output, like the lens, the bulb, or a set of LEDs. There is, however, an increasing number of fixtures on the market that, although treated as a single fixture, have multiple light output devices, i.e. heads.

For example, you might have a RGB LED bar fixture that is assembled onto a single chassis and as such it appears as a single fixture with one DMX input and one DMX output. However, it is actually comprised of four separate RGB LED "fixtures". These separate fixtures are treated in QLC+ as heads; they share some properties with their sibling heads, they can be controlled individually, but they might also have a master intensity control that controls the light output of all the heads together.

Each head belongs to a [Fixture Mode](#fixture-mode) because in one mode, a fixture might provide enough channels to control each of its heads individually while in another mode, only a handful of channels might be provided for controlling all the heads simultaneously.

### HTP (Highest Takes Precedence)

HTP is a rule that decides what level is sent to out to a DMX universe by a channel when the channel is being controlled by more than one [function](#functions) or Virtual Console widget. Generally, intensity channels obey the HTP rule. This includes generic intensity channels used to control _light intensity_ with dimmers and also channels controlling the intensity of a color, typically in an LED fixture.

The HTP rule is simple: the highest level (nearer 100%) that is currently being sent to a channel is the one that gets sent out to the DMX universe.

Let's say you have two sliders that control the same intensity channel. First, you set slider 1 to 50% and then move slider 2 from 0% to 75%. As long as slider 2 is below 50% nothing happens, but after crossing the 50% level set by slider 1, the light intensity increases up to 75%. If you drag slider 2 again towards 0%, the light intensity decreases until it reaches the 50% set by slider 1 and stays at 50% until slider 1 is dragged down.

A crossfade between 2 [Scenes](#scene) will replace the HTP levels in the first scene with the HTP levels of the second. The new HTP levels will be combined with HTP levels from other functions and virtual console widgets as above. See also [LTP](#ltp-latest-takes-precedence).

### ![](../inputoutput.svg) Input/Output plugins

QLC+ supports a variety of plugins to send and receive data from/to the external world.  
A plugin can be an interface to physical devices (such as DMX adapters or MIDI controllers) or to a network protocol (such as [Art-Net](/plugins/art-net), [OSC](/plugins/osc) or [E1.31](/plugins/e1-31-sacn)).  
Plugins support input, output or feedback capabilities depending on the device or the protocol they're controlling.  

The primary input methods for QLC+ are naturally the keyboard and mouse. Users can assign keyboard keys to virtual console buttons and drag sliders and do pretty much everything with a mouse.

Although, with plugins it is possible to attach additional input devices to one's computer to alleviate the rather clumsy and slow user experience that is achieved with a regular mouse and a keyboard. Plugins supporting an input line provide capabilities for getting external devices to produce input data to various QLC+ elements.

An input line is a connection provided by some hardware or network which is accessed through an input plugin. It can be, for example, a MIDI IN connector in the user's computer (or peripheral) to which users can connect MIDI-capable input devices like slider boards etc.

An output line is a connection provided by a hardware or network which is accessed through an output plugin. In other words, it is a real DMX universe, but has been dubbed output to separate it from QLC+'s internal universes. You could think of them as individual XLR output connectors in your DMX hardware.

### Input profiles

Input profiles can be thought of as [fixtures'](#fixtures) cousins; they contain information on specific devices that produce input data. An input device can be, for example, a slider board like the Behringer BCF-2000, KORG nanoKONTROL, an Enttec Playback Wing...

### LTP (Latest Takes Precedence)

LTP is a rule that decides what level is sent to out to a DMX universe by a channel when the channel is being controlled by more than one [function](#functions) or Virtual Console widget. Generally, it is used for channels that have been assigned to groups other than the **Intensity** group, such as pan, tilt, gobo, strobe speed and other _intelligent fixture parameters_

The LTP rule is simple: the latest level that has been set by a function or a Virtual Console widget gets sent out to the DMX universe.

During a crossfade between [Scenes](#scene), LTP levels will often be changed. This has to be handled with some care as some LTP levels need to jump immediately to a new level, for example, changing from one gobo to another. LTP groups such as pan and tilt, however, might need to change gradually from one level to another during a crossfade. Different timings can be achieved by combining scenes in a [Collection](#collection). See also [HTP](#htp-highest-takes-precedence).

### ![](../palette.svg) Palette

A Palette is an entity in QLC+ representing a fixture feature. For example a Palette can be a color, a position, a zoom angle and so on.
Palettes can be used into [Scenes](#scene) to abstract a feature regardless of the Fixtures controlled by the Scene.

### ![](../rgbmatrix.svg) RGB Matrix

An RGB matrix [function](#functions) can be used to impose simple graphics and text on a matrix (a grid or a wall) of RGB and/or monochrome fixture [heads](#head). The RGB matrix function has been designed to be extendable with [scripts](#rgb-script) that can be written by users.

Each RGB matrix has its own speed settings:

*   **Fade In:** Time to fade each pixel ON
*   **Fade Out:** Time to fade each pixel OFF
*   **Duration:** The duration of the current step/frame

### ![](../rgbmatrix.svg) RGB Script

A RGB script is a program written in [ECMAScript](https://en.wikipedia.org/wiki/ECMAScript) (also known as JavaScript) that produces the necessary image data for [RGB Matrix](#rgb-matrix) functions. Learn more from the [RGB Script API](/function-manager/rgb-script-api) page.

### ![](../scene.svg) Scene

A scene [function](#functions) comprises the values of selected channels that are contained in one or more fixture instances. When a scene is started, the time it takes for its channels to reach their target values depends on the scene's speed settings:

Each function has its own speed settings:

*   **Fade In:** The time used to fade all channels to their target values, from whatever value they had
*   **Fade Out:** The time used to fade HTP/intensity channels back to zero. Note that ONLY [HTP](#htp-highest-takes-precedence) channels are affected by this setting.

Copies of scene functions can be created with the [Function Manager](/function-manager). All of the scene's contents are copied to the duplicate.

### ![](../sequence.svg) Sequence

A Sequence has some of the functionality of a [Chaser](#chaser).  
It is equivalent to a Chaser in which each step is a single [Scene](#scene) and every one of those Scenes controls the same set of channels. A Sequence is bound to one specific Scene, which means that all the steps of the Sequence can only control the enabled channels of that Scene.  
When creating new steps in a Sequence, no Function selection pop-up will appear, since a Sequence step cannot include other Functions, unlike a Chaser step.  
When a Sequence is created, a special sequence icon will appear in the [Function Manager](/function-manager) as a child of the Scene to which it is bound.  
To understand the difference between a Sequence and a Chaser, you are invited to read the second paragraph of the [Show Manager](/show-manager) documentation.

### ![](../script.svg) Script

The Script [function](#functions) works on a simple yet powerful scripting language to automate QLC+ functionalities in a sequential order. A Script can be modified with the [Script Editor](/function-manager/script-editor).

### ![](../show.svg) Show

A Show is an advanced [function](#functions) which encapsulates most of the QLC+ Functions to create a time driven light show. A Show can be created only with the [Show Manager](/show-manager) and can be inspected and renamed with the [Show Editor](/function-manager/show-editor).

### ![](../video2.svg) Video

A video [function](#functions) is an object representing a video file stored in a disk or a network URL.  
The supported video formats depends on your Operating System. For example Mac OSX is limited to MOV/MP4 files and not much more.  
Video functions can be placed in [Chaser](#chaser) or in a [Show](#show) at the desired time, using the [Show Manager](/show-manager) panel.
