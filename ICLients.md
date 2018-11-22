# Описание интерфейса IClient
Интерфейс предназначен для работы с методами класса Client

## Реализация интерфейса
* +AddClient (Client:[Client](https://github.com/polinanch/Documents/blob/master/Client.md "объект класса Clients")): Int — функция, добавляющая клиента в базу данных. Параметр «[Client](ссылка "объект класса Client")» — клиент, 
который необходимо добавить в БД;
* +EditClient (Client:[Client](https://github.com/polinanch/Documents/blob/master/Client.md "объект класса Client")): Bool — функция, редактирующая данные о клиенте. Параметр «Client:[Client](https://github.com/gogganesko/Orho/blob/master/docs/Clients.md "объект класса Client")» — 
клиента, которого необходимо редактировать в БД;
* +FindByID(ID: Int): [Client](https://github.com/polinanch/Documents/blob/master/Client.md "объект класса Client")  — функция, осуществляющая поиск клиента в базе данных по ID и возвращающая найденный, если такой есть. 
* +Del(ID): Bool – функция удаляет клиента.
* +Getchedule(ID : int) : List <[Schedule](https://github.com/polinanch/Documents/blob/master/Schedule.md "объект класса Schedule")> - функция возвращающая расписание клиента.
* +GetAllCourses(ID : int) : List <[Course](https://github.com/polinanch/Documents/blob/master/Course.md "объект класса Courses")> - функция возвращает список курсов данного клиента.
* +GetAllGroup(ID : int) : List <[Groups](https://github.com/polinanch/Documents/blob/master/Group.md "объект класса Groups")> - функция возвращает список групп данного клиента.
* +GetAllLanguage(ID : int) :  List <[Language](https://github.com/polinanch/Documents/blob/master/Language.md "объект класса Language")> - функция возвращает список изучаемых языков 
 данного клиента.
 * +GetAllClients(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Client](https://github.com/polinanch/Documents/blob/master/Client.md "объект класса Client")> — функция, возвращающая список клиентов. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
