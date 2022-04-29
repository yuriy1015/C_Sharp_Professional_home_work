# My homework for the C# Professional course

## less-01_pro_UserCollection
1. Create a method that takes an array of integers as an argument and returns
   collection of squares of all odd numbers in the array. Use the yield statement to form a collection.
2. Create a collection that would store the names of 12 months, the serial number and
   the number of days in the corresponding month. Implement the ability to select months, as in
   serial number, and the number of days in a month, while the result can be not only one month.
3. Create an abstract class Citizen. Create classes Student, Retired, Worker
   inherited from Citizen. Create a non-parameterized collection with the following functionality:
    1. Adding an element to the collection.
      1) You can only add a Citizen.
      2) When adding, the element is added to the end of the collection. If Retired, then in
         start taking into account the previously standing Pensioners. The number in the queue is returned.
      3) When adding the same person (check for equality by number
         passport, you need to override the Equals method and/or the equality operators to
         comparison of objects by passport number) the element is not added, a message is displayed.
    2. Removal
      1) Deletion - from the beginning of the collection.
      2) It is possible to delete with the transfer of a copy of the Citizen.
    3. The Contains method returns true/false if the element is present/absent in the collection and the number in the queue.
    4. The ReturnLast method returns the last person in the queue and their number in the queue.
    5. The Clear method clears the collection.
    6. You can work with the collection using the foreach operator.

## less-02_pro_SysCollection
1. Using the SortedList class, create a small collection and display the values ??of key-value pairs
    first in alphabetical order and then in reverse.
2. Create a collection where you can add customers and the category they purchased
    products. From the collection, you can get categories of goods that the buyer bought or
    categories define buyers.
3. In several ways, create a collection that can store only integers and
    real values, according to the type "company account - available amount", respectively.
4. Create a collection of type OrderedDictionary and implement the ability to compare key values ??in it.

## less-03_pro_IO
1. Create 100 directories on disk named Folder_0 to Folder_99, then delete them.
2. Create a file, write arbitrary data to it, and close the file. Then reopen
    this file, read data from it and print it to the console.
3. Write an application to search for a given file on disk. Add code using
    class FileStream and allows you to view the file in a text window. In conclusion
    add the ability to compress the found file.
4 Create a WPF Application that allows users to save data to isolated storage.
    This task requires the presence of the Xceed.Wpf.Toolkit.dll library. Her
    can be obtained through References -> Manage NuGet Packages... -> in the search write Extended
    WPF Toolkit (in addition to the library we are interested in, others will be installed), or
    download directly on the site http://wpftoolkit.codeplex.com/ and connect to the project only
    the library we are interested in (References -> Add Reference ...).
        1. Place a Label and a Button in the window.
        2. Place in the ColorPicker window (this tool is provided by the above
library). To do this, in the XAML code in the Window tag, connect the space
names xmlns:xctk="http://schemas.xceed.com/wpf/xaml/toolkit" . Also, we need an event
Loaded windows.
3. Implement so that when a color is selected from the ColorPicker, the name is displayed in the Label
the selected color and the background of the Label was painted in this color. At the push of a button, information about
colors are stored in isolated storage. When you start the application again, the background color
The Label remains the same as it was saved on previous runs of the application.

## less-04_pro_TXT
1. Write a console application that allows the user to register under
    "Login", consisting only of characters of the Latin alphabet, and a password, consisting of numbers and symbols.
2. Write a program that would allow you to the specified address of a web page
    select all links to other pages, phone numbers, postal addresses and save the result to a file.
3. Write a joke program "Decoder" that could replace all prepositions in a text file with the word "GAV!".
4. Create a text file-receipt of the type "Product name - 0.00 (price) UAH." with
    a certain number of items of goods and the date of the purchase.Display on
    screen information from the receipt in the format of the user's current locale and in the en-US locale format.

## less-05_pro_XML
1. Create an .xml file that meets the following requirements:
    - filename: TelephoneBook.xml
    - root element: “MyContacts”
    - tag “Contact”, and it should contain the name of the contact and the attribute “TelephoneNumber” with the value of the phone number.
2. Create an application that displays all the information about the specified .xml file.
3. From the TelephoneBook.xml file (the file must have been created during an additional task), output
    only phone numbers appear on the screen.
4. Create a WPF Application, in the main window of which place any text. Also,
    there should be a settings window (can be implemented using TabControl). The user can
    change settings. When you restart the application, the settings should remain the same.
    Implement two options (in one application or two different ones):
1) saving settings in the configuration file;
2) saving settings in the registry.
    In the settings window, implement the following options: background color, text color, font size, font style, and a button
    "Save". To select a color, use the ColorPicker, following the example of the task from Lesson #3.

## less-06_pro_Reflection
1. Create a reflector program that will allow you to get information about the assembly and incoming
    in its composition types. For the basis, you can use the reflector program from the lesson.
2. Create your custom assembly following the CarLibrary assembly example from the lesson, the assembly will be
    be used with a temperature converter.
3. Create a program where you give the user access to the assembly from Task 2.
    Implement a method to convert a temperature value from Celsius to Fahrenheit.
    When doing the task, use only reflection.

## less-07_pro_Attributes
1. Create a custom AccessLevelAttribute to define
    level of user access to the system. Form the composition of employees of a certain company
    as a set of classes, for example, Manager, Programmer, Director. Using the attribute
    AccessLevelAttribute allocate personnel access levels and display
    reaction of the system to each employee's attempt to gain access to the protected section.
2. Create a class and apply the Obsolete attribute to its methods first in the form, simply
    outputting a warning, and then in a form that prevents compilation.
    Demonstrate how the attribute works by calling these methods as an example.
3. Expand the capabilities of the reflector program from the previous lesson as follows:
      1. Add the ability to choose which members of the type should be shown
         user. At the same time, it should be possible to select several members at once
         type, such as methods and properties.
     2. Add the ability to display information about attributes for types and all members of the type,
         which can be decorated with attributes.

## less-08_pro_Serialization
1. Create a custom type (like a class) and serialize an object of that
    type, given the fact that the state of the object will need to be transmitted over the network.
2. Create a class that supports serialization. Serialize the object of this
    class in XML format. First use the default format and then change it
    so that the field values ??are stored as attributes of the XML elements.
3. Create a new application in which you deserialize the object from the previous example.
    Display the state of the object on the screen.

## less-09_pro_ GarbageCollector
1. Create your own class whose objects will take up a lot of memory space (for example, in
    there will be a large array in the class code) and implement a formalized cleanup pattern for this class.
2. Create a class that will allow you to monitor the resources used by the program.
    Use it to monitor the operation of the program, namely: the user can
    specify acceptable levels of resource (memory) consumption, and class methods will allow you to issue
    a warning when the amount of actually used resources approaches the maximum allowable level.

## less-10_pro_Version
1. Implement the NVI pattern in your own inheritance hierarchy.
2. Learn the description of the Template Method template. pay attention to
    the applicability of the template, as well as the composition of its participants and the relationship of the relationship between them.
    Write a small C# program that is an abstract implementation of this pattern.

## less-11_pro_Thread_1
1. Using blocking constructs, create a method that will be in the for loop (say, at 10
    iterations) increment the counter by one and display the counter and the current thread.
    The method is run in three threads. Each thread must be executed in turn, i.e. in
    As a result, numbers (counter values) from 1 to 30 should be displayed on the screen in order, and not in
    random order.
2. Create a console application that in different threads can access 2
    files. Read the contents of these files and try to write the resulting
    information to the third file. Reading / writing must be carried out simultaneously in each
    from child threads. Use thread blocking to achieve correct
    writing to the final file.

## less-12_pro_Thread_2
1. Create a Semaphore that controls access to a resource from multiple threads.
    Organize an ordered output of information about obtaining access to a special *.log file.
2. Convert the event blocking example so that automatic processing is used instead of manual processing.
3. Create an application that can only run in one instance (using a named Mutex).

## less-13_pro_Async
1. Create a WPF application. On the main form of the application, place 3 buttons with
    names: IsComplete, End, Callback. Organize button click handlers like this
    so that they initiate the asynchronous execution of some method (method
    determine for yourself, you can use something like Add or the more abstract Compute).
    For each of the buttons, the completion of the async method should be tracked accordingly:
- IsComplete - using the value of the IsComplete property
- End - just by applying EndInvoke
- Callback - using the callback method
2. Create a console application in which organize an asynchronous method call.
    Using the BeginInvoke construct, pass some information to the thread (perhaps in
    string format). Organize the processing of the transferred data in the callback method.

## less-14_pro_Task_Parallel_Library
1. Create an array of numbers with dimensions of 1,000,000 or more. Using a random number generator, initialize this
    array of values. Create a PLINQ query that will allow you to get all the odd numbers from the original array.
2. Create two methods that will be executed as part of parallel tasks. Arrange to call these methods when
    help Invoke so that the main thread of the program (the Main method) does not stop its execution.

## less-15_pro_Async_ Await
1. Redo the extra task from Lesson 11 using the async await construct.
2. Create a WPF application, place two buttons in the TextBox window. By clicking on the first
    button in the TextBox, the message "Connected to the database" is displayed, while in the handler
    set a delay of 3-5 seconds to simulate a connection to the database, this button also launches
    a timer that, at intervals of several seconds, displays the message “Data
    received." When you press the second button, by analogy with the first, we disconnect from the base (with
    delay), display a message and stop the timer.


# Мои домашние задания по курсу C# Professional

## less-01_pro_UserCollection
1. Создайте метод, который в качестве аргумента принимает массив целых чисел и возвращает
   коллекцию квадратов всех нечетных чисел массива.Для формирования коллекции  используйте оператор yield.
2. Создайте коллекцию, в которой бы хранились наименования 12 месяцев, порядковый номер и
   количество дней в соответствующем месяце.Реализуйте возможность выбора месяцев, как по
   порядковому номеру, так и количеству дней в месяце, при этом результатом может быть не только один месяц.
3. Создайте абстрактный класс Гражданин. Создайте классы Студент, Пенсионер, Рабочий
   унаследованные от Гражданина.Создайте непараметризированную коллекцию со следующим функционалом:
    1. Добавление элемента в коллекцию.
      1) Можно добавлять только Гражданина.
      2) При добавлении, элемент добавляется в конец коллекции.Если Пенсионер, – то в
         начало с учетом ранее стоящих Пенсионеров. Возвращается номер в очереди.
      3) При добавлении одного и того же человека(проверка на равенство по номеру
         паспорта, необходимо переопределить метод Equals и/или операторы равенства для
         сравнения объектов по номеру паспорта) элемент не добавляется, выдается сообщение.
    2. Удаление
      1) Удаление – с начала коллекции.
      2) Возможно удаление с передачей экземпляра Гражданина.
    3. Метод Contains возвращает true/false при налчичии/отсутствии элемента в коллекции и  номер в очереди.
    4. Метод ReturnLast возвращsает последнего чеолвека в очереди и его номер в очереди.
    5. Метод Clear очищает коллекцию.
    6. С коллекцией можно работать опертаором foreach.

## less-02_pro_SysCollection
1.  Используя класс SortedList, создайте небольшую коллекцию и выведите на экран значения пар «ключ- значение» 
    сначала в алфавитном порядке, а затем в обратном.
2.  Создайте коллекцию, в которую можно добавлять покупателей и категорию приобретенной ими
    продукции.Из коллекции можно получать категории товаров, которые купил покупатель или по
    категории определить покупателей.
3.  Несколькими способами создайте коллекцию, в которой можно хранить только целочисленные и
    вещественные значения, по типу «счет предприятия – доступная сумма» соответственно.
4.  Создайте коллекцию типа OrderedDictionary и реализуйте в ней возможность сравнения значений ключей.

## less-03_pro_IO
1.  Создайте на диске 100 директорий с именами от Folder_0 до Folder_99, затем удалите их.
2.  Создайте файл, запишите в него произвольные данные и закройте файл. Затем снова откройте
    этот файл, прочитайте из него данные и выведете их на консоль.
3.  Напишите приложение для поиска заданного файла на диске. Добавьте код, использующий
    класс FileStream и позволяющий просматривать файл в текстовом окне.В заключение
    добавьте возможность сжатия найденного файла.
4.  Создайте приложение WPF Application, позволяющее пользователям сохранять данные в изолированное хранилище.
    Для выполнения этого задания необходимо наличие библиотеки Xceed.Wpf.Toolkit.dll. Ее
    можно получить через References -> Manage NuGet Packages… -> в поиске написать Extended
    WPF Toolkit (помимо интересующей нас библиотеки будут установлены и другие), или же
    скачать непосредственно на сайте http://wpftoolkit.codeplex.com/ и подключить в проект только
    интересующую нас бибилиотеку (References -> Add Reference …).
        1. Разместите в окне Label и Button.
        2. Разместите в окне ColorPicker (данный инструмент предоставляется вышеуказанной
	библиотекой). Для этого необходимо в XAML коде в теге Window подключить пространство
	имен xmlns:xctk="http://schemas.xceed.com/wpf/xaml/toolkit" . Также, нам понадобиться событие
	Loaded окна.
	3. Реализуйте, чтобы при выборе цвета из ColorPicker в Label выводилось название
	выбранного цвета и в этот цвет закрашивался фон Label. По нажатию на кнопку, данные о
	цвете сохраняются в изолированное хранилище. При запуске приложения заново, цвет фона
	Label остается таким, каким был сохранен при предыдущих запусках приложения.

## less-04_pro_TXT
1.  Напишите консольное приложение, позволяющие пользователю зарегистрироваться под
    «Логином», состоящем только из символов латинского алфавита, и пароля, состоящего из цифр и символов.
2.  Напишите программу, которая бы позволила вам по указанному адресу web-страницы
    выбирать все ссылки на другие страницы, номера телефонов, почтовые адреса и сохраняла полученный результат в файл.
3.  Напишите шуточную программу «Дешифратор», которая бы в текстовом файле могла бы заменить все предлоги на слово «ГАВ!».
4.  Создайте текстовый файл-чек по типу «Наименование товара – 0.00 (цена) грн.» с
    определенным количеством наименований товаров и датой совершения покупки.Выведите на
    экран информацию из чека в формате текущей локали пользователя и в формате локали en-US.

## less-05_pro_XML
1.  Создайте .xml файл, который соответствовал бы следующим требованиям:
    - имя файла: TelephoneBook.xml
    - корневой элемент: “MyContacts”
    - тег “Contact”, и в нем должно быть записано имя контакта и атрибут “TelephoneNumber” со значением номера телефона.
2.  Создайте приложение, которое выводит на экран всю информацию об указанном .xml файле.
3.  Из файла TelephoneBook.xml (файл должен был быть создан в процессе выполнения дополнительного задания) выведите 
    на экран только номера телефонов.
4.  Создайте приложение WPF Application, в главном окне которого поместите любой текст. Также,
    должно быть окно настроек (можно реализовать с помощью TabControl). Пользователь может
    изменять настройки. При повторном запуске приложения настройки должны оставаться прежними. 
    Реализуйте два варианта (в одном приложении или двух разных): 
	1) сохранение настроек в конфигурационном файле; 
	2) сохранение настроек в реестре.
    В окне настроек реализуйте следующие опции: цвет фона, цвет текста, размер шрифта, стиль шрифта, а также кнопку 
    «Сохранить». Для выбора цвета воспользуйтесь ColorPicker-ом по примеру задания из Урока №3.

## less-06_pro_Reflection
1.  Создайте программу-рефлектор, которая позволит получить информацию о сборке и входящих
    в ее состав типах.Для основы можно использовать программу-рефлектор из урока.
2.  Создайте свою пользовательскую сборку по примеру сборки CarLibrary из урока, сборка будет
    использоваться для работы с конвертером температуры.
3.  Создайте программу, в которой предоставьте пользователю доступ к сборке из Задания 2.
    Реализуйте использование метода конвертации значения температуры из шкалы Цельсия в шкалу Фаренгейта.
    Выполняя задание используйте только рефлексию.

## less-07_pro_Attributes
1.  Создайте пользовательский атрибут AccessLevelAttribute, позволяющий определить
    уровень доступа пользователя к системе.Сформируйте состав сотрудников некоторой фирмы
    в виде набора классов, например, Manager, Programmer, Director.При помощи атрибута
    AccessLevelAttribute распределите уровни доступа персонала и отобразите на экране
    реакцию системы на попытку каждого сотрудника получить доступ в защищенную секцию.
2.  Создайте класс и примените к его методам атрибут Obsolete сначала в форме, просто
    выводящей предупреждение, а затем в форме, препятствующей компиляции.
    Продемонстрируйте работу атрибута на примере вызова данных методов.
3.  Расширьте возможности программы-рефлектора из предыдущего урока следующим образом:
      1. Добавьте возможность выбирать, какие именно члены типа должны быть показаны
         пользователю.При этом должна быть возможность выбирать сразу несколько членов
         типа, например, методы и свойства.
     2.  Добавьте возможность вывода информации об атрибутах для типов и всех членов типа,
         которые могут быть декорированы атрибутами.

## less-08_pro_Serialization
1.  Создайте пользовательский тип (например, класс) и выполните сериализацию объекта этого
    типа, учитывая тот факт, что состояние объекта необходимо будет передать по сети.
2.  Создайте класс, поддерживающий сериализацию. Выполните сериализацию объекта этого
    класса в формате XML. Сначала используйте формат по умолчанию, а затем измените его
    таким образом, чтобы значения полей сохранились в виде атрибутов элементов XML.
3.  Создайте новое приложение, в котором выполните десериализацию объекта из предыдущего примера. 
    Отобразите состояние объекта на экране.

## less-09_pro_ GarbageCollector
1.  Создайте свой класс, объекты которого будут занимать много места в памяти (например, в
    коде класса будет присутствовать большой массив) и реализуйте для этого класса, формализованный шаблон очистки.
2.  Создайте класс, который позволит выполнять мониторинг ресурсов, используемых программой.
    Используйте его в целях наблюдения за работой программы, а именно: пользователь может
    указать приемлемые уровни потребления ресурсов(памяти), а методы класса позволят выдать
    предупреждение, когда количество реально используемых ресурсов приблизиться к максимально допустимому уровню.

## less-10_pro_Version
1.  Реализуйте шаблон NVI в собственной иерархии наследования.
2.  Выучите описание шаблона Template method (Шаблонный метод). Обратите внимание на
    применимость шаблона, а также на состав его участников и связи отношения между ними.
    Напишите небольшую программу на языке C#, представляющую собой абстрактную реализацию данного шаблона.

## less-11_pro_Thread_1
1.  Используя конструкции блокировки, создайте метод, который будет в цикле for (допустим, на 10
    итераций) увеличивать счетчик на единицу и выводить на экран счетчик и текущий поток.
    Метод запускается в трех потоках. Каждый поток должен выполниться поочередно, т.е.в
    результате на экран должны выводиться числа (значения счетчика) с 1 до 30 по порядку, а не в
    произвольном порядке.
2.  Создайте консольное приложение, которое в различных потоках сможет получить доступ к 2-м
    файлам.Считайте из этих файлов содержимое и попытайтесь записать полученную
    информацию в третий файл.Чтение/запись должны осуществляться одновременно в каждом
    из дочерних потоков.Используйте блокировку потоков для того, чтобы добиться корректной
    записи в конечный файл.

## less-12_pro_Thread_2
1.  Создайте Semaphore, осуществляющий контроль доступа к ресурсу из нескольких потоков.
    Организуйте упорядоченный вывод информации о получении доступа в специальный*.log  файл.
2.  Преобразуйте пример событийной блокировки таким образом, чтобы вместо ручной обработки использовалась автоматическая.
3.  Создайте приложение, которое может быть запущено только в одном экземпляре (используя именованный Mutex).

## less-13_pro_Async
1.  Создайте WPF приложение. На главной форме приложения разместите 3 кнопки с
    названиями: IsComplete, End, Callback. Организуйте обработчики нажатия на кнопки таким
    образом, чтобы они инициировали асинхронное выполнение некоторого метода (метод
    определите сами, можно воспользоваться чем-то вроде Add или более абстрактного Compute).
    Для каждой из кнопок завершение асинхронного метода должно отслеживаться соответствующим образом:
	- IsComplete – с использованием значения свойства IsComplete
	- End – просто применяя EndInvoke
	- Callback – с использованием callback метода
2.  Создайте консольное приложение, в котором организуйте асинхронный вызов метода.
    Используя конструкцию BeginInvoke передайте в поток некоторую информацию (возможно, в
    формате строки). Организуйте обработку переданных данных в callback методе.

## less-14_pro_Task_Parallel_Library
1.  Создайте массив чисел размерностью в 1 000 000 или более. Используя генератор случайных чисел, проинициализируйте этот 
    массив значениями. Создайте PLINQ запрос, который позволит получить все нечетные числа из исходного массива.
2.  Создайте два метода, которые будут выполняться в рамках параллельных задач. Организуйте вызов этих методов при 
    помощи Invoke таким образом, чтобы основной поток программы (метод Main) не остановил свое выполнение.

## less-15_pro_Async_ Await
1.  Переделайте дополнительное задание из урока №11 с использованием конструкции async await.
2.  Создайте WPF приложение, разместите в окне TextBox и две кнопки. При нажатии на первую
    кнопку в TextBox выводится сообщение «Подключен к базе данных» при этом в обработчике
    установите задержку в 3-5 сек для имитации подключения к БД, также данная кнопка запускает
    таймер, который с периодичностью в несколько секунд выводит в TextBox сообщение «Данные
    получены». При нажатии на вторую кнопку по аналогии с первой отключаемся от базы (с
    задержкой), выводим сообщение и останавливаем таймер.
