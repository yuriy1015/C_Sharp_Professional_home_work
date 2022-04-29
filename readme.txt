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
    - root element: �MyContacts�
    - tag �Contact�, and it should contain the name of the contact and the attribute �TelephoneNumber� with the value of the phone number.
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
    a timer that, at intervals of several seconds, displays the message �Data
    received." When you press the second button, by analogy with the first, we disconnect from the base (with
    delay), display a message and stop the timer.


# ��� �������� ������� �� ����� C# Professional

## less-01_pro_UserCollection
1. �������� �����, ������� � �������� ��������� ��������� ������ ����� ����� � ����������
   ��������� ��������� ���� �������� ����� �������.��� ������������ ���������  ����������� �������� yield.
2. �������� ���������, � ������� �� ��������� ������������ 12 �������, ���������� ����� �
   ���������� ���� � ��������������� ������.���������� ����������� ������ �������, ��� ��
   ����������� ������, ��� � ���������� ���� � ������, ��� ���� ����������� ����� ���� �� ������ ���� �����.
3. �������� ����������� ����� ���������. �������� ������ �������, ���������, �������
   �������������� �� ����������.�������� ��������������������� ��������� �� ��������� ������������:
    1. ���������� �������� � ���������.
      1) ����� ��������� ������ ����������.
      2) ��� ����������, ������� ����������� � ����� ���������.���� ���������, � �� �
         ������ � ������ ����� ������� �����������. ������������ ����� � �������.
      3) ��� ���������� ������ � ���� �� ��������(�������� �� ��������� �� ������
         ��������, ���������� �������������� ����� Equals �/��� ��������� ��������� ���
         ��������� �������� �� ������ ��������) ������� �� �����������, �������� ���������.
    2. ��������
      1) �������� � � ������ ���������.
      2) �������� �������� � ��������� ���������� ����������.
    3. ����� Contains ���������� true/false ��� ��������/���������� �������� � ��������� �  ����� � �������.
    4. ����� ReturnLast �������s��� ���������� �������� � ������� � ��� ����� � �������.
    5. ����� Clear ������� ���������.
    6. � ���������� ����� �������� ���������� foreach.

## less-02_pro_SysCollection
1.  ��������� ����� SortedList, �������� ��������� ��������� � �������� �� ����� �������� ��� �����- �������� 
    ������� � ���������� �������, � ����� � ��������.
2.  �������� ���������, � ������� ����� ��������� ����������� � ��������� ������������� ���
    ���������.�� ��������� ����� �������� ��������� �������, ������� ����� ���������� ��� ��
    ��������� ���������� �����������.
3.  ����������� ��������� �������� ���������, � ������� ����� ������� ������ ������������� �
    ������������ ��������, �� ���� ����� ����������� � ��������� ����� ��������������.
4.  �������� ��������� ���� OrderedDictionary � ���������� � ��� ����������� ��������� �������� ������.

## less-03_pro_IO
1.  �������� �� ����� 100 ���������� � ������� �� Folder_0 �� Folder_99, ����� ������� ��.
2.  �������� ����, �������� � ���� ������������ ������ � �������� ����. ����� ����� ��������
    ���� ����, ���������� �� ���� ������ � �������� �� �� �������.
3.  �������� ���������� ��� ������ ��������� ����� �� �����. �������� ���, ������������
    ����� FileStream � ����������� ������������� ���� � ��������� ����.� ����������
    �������� ����������� ������ ���������� �����.
4.  �������� ���������� WPF Application, ����������� ������������� ��������� ������ � ������������� ���������.
    ��� ���������� ����� ������� ���������� ������� ���������� Xceed.Wpf.Toolkit.dll. ��
    ����� �������� ����� References -> Manage NuGet Packages� -> � ������ �������� Extended
    WPF Toolkit (������ ������������ ��� ���������� ����� ����������� � ������), ��� ��
    ������� ��������������� �� ����� http://wpftoolkit.codeplex.com/ � ���������� � ������ ������
    ������������ ��� ����������� (References -> Add Reference �).
        1. ���������� � ���� Label � Button.
        2. ���������� � ���� ColorPicker (������ ���������� ��������������� �������������
	�����������). ��� ����� ���������� � XAML ���� � ���� Window ���������� ������������
	���� xmlns:xctk="http://schemas.xceed.com/wpf/xaml/toolkit" . �����, ��� ������������ �������
	Loaded ����.
	3. ����������, ����� ��� ������ ����� �� ColorPicker � Label ���������� ��������
	���������� ����� � � ���� ���� ������������ ��� Label. �� ������� �� ������, ������ �
	����� ����������� � ������������� ���������. ��� ������� ���������� ������, ���� ����
	Label �������� �����, ����� ��� �������� ��� ���������� �������� ����������.

## less-04_pro_TXT
1.  �������� ���������� ����������, ����������� ������������ ������������������ ���
    ��������, ��������� ������ �� �������� ���������� ��������, � ������, ���������� �� ���� � ��������.
2.  �������� ���������, ������� �� ��������� ��� �� ���������� ������ web-��������
    �������� ��� ������ �� ������ ��������, ������ ���������, �������� ������ � ��������� ���������� ��������� � ����.
3.  �������� �������� ��������� �����������, ������� �� � ��������� ����� ����� �� �������� ��� �������� �� ����� ����!�.
4.  �������� ��������� ����-��� �� ���� ������������� ������ � 0.00 (����) ���.� �
    ������������ ����������� ������������ ������� � ����� ���������� �������.�������� ��
    ����� ���������� �� ���� � ������� ������� ������ ������������ � � ������� ������ en-US.

## less-05_pro_XML
1.  �������� .xml ����, ������� �������������� �� ��������� �����������:
    - ��� �����: TelephoneBook.xml
    - �������� �������: �MyContacts�
    - ��� �Contact�, � � ��� ������ ���� �������� ��� �������� � ������� �TelephoneNumber� �� ��������� ������ ��������.
2.  �������� ����������, ������� ������� �� ����� ��� ���������� �� ��������� .xml �����.
3.  �� ����� TelephoneBook.xml (���� ������ ��� ���� ������ � �������� ���������� ��������������� �������) �������� 
    �� ����� ������ ������ ���������.
4.  �������� ���������� WPF Application, � ������� ���� �������� ��������� ����� �����. �����,
    ������ ���� ���� �������� (����� ����������� � ������� TabControl). ������������ �����
    �������� ���������. ��� ��������� ������� ���������� ��������� ������ ���������� ��������. 
    ���������� ��� �������� (� ����� ���������� ��� ���� ������): 
	1) ���������� �������� � ���������������� �����; 
	2) ���������� �������� � �������.
    � ���� �������� ���������� ��������� �����: ���� ����, ���� ������, ������ ������, ����� ������, � ����� ������ 
    �����������. ��� ������ ����� �������������� ColorPicker-�� �� ������� ������� �� ����� �3.

## less-06_pro_Reflection
1.  �������� ���������-���������, ������� �������� �������� ���������� � ������ � ��������
    � �� ������ �����.��� ������ ����� ������������ ���������-��������� �� �����.
2.  �������� ���� ���������������� ������ �� ������� ������ CarLibrary �� �����, ������ �����
    �������������� ��� ������ � ����������� �����������.
3.  �������� ���������, � ������� ������������ ������������ ������ � ������ �� ������� 2.
    ���������� ������������� ������ ����������� �������� ����������� �� ����� ������� � ����� ����������.
    �������� ������� ����������� ������ ���������.

## less-07_pro_Attributes
1.  �������� ���������������� ������� AccessLevelAttribute, ����������� ����������
    ������� ������� ������������ � �������.����������� ������ ����������� ��������� �����
    � ���� ������ �������, ��������, Manager, Programmer, Director.��� ������ ��������
    AccessLevelAttribute ������������ ������ ������� ��������� � ���������� �� ������
    ������� ������� �� ������� ������� ���������� �������� ������ � ���������� ������.
2.  �������� ����� � ��������� � ��� ������� ������� Obsolete ������� � �����, ������
    ��������� ��������������, � ����� � �����, �������������� ����������.
    ����������������� ������ �������� �� ������� ������ ������ �������.
3.  ��������� ����������� ���������-���������� �� ����������� ����� ��������� �������:
      1. �������� ����������� ��������, ����� ������ ����� ���� ������ ���� ��������
         ������������.��� ���� ������ ���� ����������� �������� ����� ��������� ������
         ����, ��������, ������ � ��������.
     2.  �������� ����������� ������ ���������� �� ��������� ��� ����� � ���� ������ ����,
         ������� ����� ���� ������������ ����������.

## less-08_pro_Serialization
1.  �������� ���������������� ��� (��������, �����) � ��������� ������������ ������� �����
    ����, �������� ��� ����, ��� ��������� ������� ���������� ����� �������� �� ����.
2.  �������� �����, �������������� ������������. ��������� ������������ ������� �����
    ������ � ������� XML. ������� ����������� ������ �� ���������, � ����� �������� ���
    ����� �������, ����� �������� ����� ����������� � ���� ��������� ��������� XML.
3.  �������� ����� ����������, � ������� ��������� �������������� ������� �� ����������� �������. 
    ���������� ��������� ������� �� ������.

## less-09_pro_ GarbageCollector
1.  �������� ���� �����, ������� �������� ����� �������� ����� ����� � ������ (��������, �
    ���� ������ ����� �������������� ������� ������) � ���������� ��� ����� ������, ��������������� ������ �������.
2.  �������� �����, ������� �������� ��������� ���������� ��������, ������������ ����������.
    ����������� ��� � ����� ���������� �� ������� ���������, � ������: ������������ �����
    ������� ���������� ������ ����������� ��������(������), � ������ ������ �������� ������
    ��������������, ����� ���������� ������� ������������ �������� ������������ � ����������� ����������� ������.

## less-10_pro_Version
1.  ���������� ������ NVI � ����������� �������� ������������.
2.  ������� �������� ������� Template method (��������� �����). �������� �������� ��
    ������������ �������, � ����� �� ������ ��� ���������� � ����� ��������� ����� ����.
    �������� ��������� ��������� �� ����� C#, �������������� ����� ����������� ���������� ������� �������.

## less-11_pro_Thread_1
1.  ��������� ����������� ����������, �������� �����, ������� ����� � ����� for (��������, �� 10
    ��������) ����������� ������� �� ������� � �������� �� ����� ������� � ������� �����.
    ����� ����������� � ���� �������. ������ ����� ������ ����������� ����������, �.�.�
    ���������� �� ����� ������ ���������� ����� (�������� ��������) � 1 �� 30 �� �������, � �� �
    ������������ �������.
2.  �������� ���������� ����������, ������� � ��������� ������� ������ �������� ������ � 2-�
    ������.�������� �� ���� ������ ���������� � ����������� �������� ����������
    ���������� � ������ ����.������/������ ������ �������������� ������������ � ������
    �� �������� �������.����������� ���������� ������� ��� ����, ����� �������� ����������
    ������ � �������� ����.

## less-12_pro_Thread_2
1.  �������� Semaphore, �������������� �������� ������� � ������� �� ���������� �������.
    ����������� ������������� ����� ���������� � ��������� ������� � �����������*.log  ����.
2.  ������������ ������ ���������� ���������� ����� �������, ����� ������ ������ ��������� �������������� ��������������.
3.  �������� ����������, ������� ����� ���� �������� ������ � ����� ���������� (��������� ����������� Mutex).

## less-13_pro_Async
1.  �������� WPF ����������. �� ������� ����� ���������� ���������� 3 ������ �
    ����������: IsComplete, End, Callback. ����������� ����������� ������� �� ������ �����
    �������, ����� ��� ������������ ����������� ���������� ���������� ������ (�����
    ���������� ����, ����� ��������������� ���-�� ����� Add ��� ����� ������������ Compute).
    ��� ������ �� ������ ���������� ������������ ������ ������ ������������� ��������������� �������:
	- IsComplete � � �������������� �������� �������� IsComplete
	- End � ������ �������� EndInvoke
	- Callback � � �������������� callback ������
2.  �������� ���������� ����������, � ������� ����������� ����������� ����� ������.
    ��������� ����������� BeginInvoke ��������� � ����� ��������� ���������� (��������, �
    ������� ������). ����������� ��������� ���������� ������ � callback ������.

## less-14_pro_Task_Parallel_Library
1.  �������� ������ ����� ������������ � 1 000 000 ��� �����. ��������� ��������� ��������� �����, ������������������ ���� 
    ������ ����������. �������� PLINQ ������, ������� �������� �������� ��� �������� ����� �� ��������� �������.
2.  �������� ��� ������, ������� ����� ����������� � ������ ������������ �����. ����������� ����� ���� ������� ��� 
    ������ Invoke ����� �������, ����� �������� ����� ��������� (����� Main) �� ��������� ���� ����������.

## less-15_pro_Async_ Await
1.  ����������� �������������� ������� �� ����� �11 � �������������� ����������� async await.
2.  �������� WPF ����������, ���������� � ���� TextBox � ��� ������. ��� ������� �� ������
    ������ � TextBox ��������� ��������� ���������� � ���� ������� ��� ���� � �����������
    ���������� �������� � 3-5 ��� ��� �������� ����������� � ��, ����� ������ ������ ���������
    ������, ������� � �������������� � ��������� ������ ������� � TextBox ��������� �������
    ���������. ��� ������� �� ������ ������ �� �������� � ������ ����������� �� ���� (�
    ���������), ������� ��������� � ������������� ������.
