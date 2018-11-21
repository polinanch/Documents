# Описание интерфейса ITeacher
Интерфейс предназначен для работы с методами класса Teacher

## Реализация интерфейса
* +AddTeacher (Teacher:[Teacher](ссылка "объект класса Teachers")): Int — функция, добавляющая преподавателя в базу данных. Параметр
 «[Teacher](ссылка "объект класса Teacher")» — преподаватель, 
которого необходимо добавить в БД;
* +EdiTeacher (Teacher:[Teacher](https://github.com/gogganesko/Orho/blob/master/docs/Teachers.md "объект класса Teacher")): Bool — функция, редактирующая
 данные о преподавателе. Параметр «Teacher:[Teacher](https://github.com/gogganesko/Orho/blob/master/docs/Teachers.md "объект класса Teacher")» — 
преподаватель, которого необходимо редактировать в БД;
* +FindByID(ID: Int): [Person](https://github.com/gogganesko/Orho/blob/master/docs/Teachers.md "объект класса Teacher")  — функция, осуществляющая 
поиск преподавателя в базе данных по ID и возвращающая найденный, если такой есть. 
* +Del(ID): Bool – функция удаляет преподавателя.
* +GetAllTeachers(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Teacher]
(https://github.com/gogganesko/Orho/blob/master/docs/Teachers.md "объект класса Teacher")> — функция, возвращающая список преподавателей. 
* +Getchedule(ID : int) : List<Schedule> - функция возвращающая расписание преподавателя.
* +GetAllCourses(ID : int) : List<Courses> - функция возвращает список курсов данного преподавателя.
* +GetAllGroup(ID : int) : List<Groups> - функция возвращает список групп данного преподавателя.
* +GetAllLanguage(ID : int) :  List<Languages> - функция возвращает список изучаемых языков данного преподавателя.
* +GetAllSalary (ID : int) : List<Salary> - функция возвращает список зарплат преподавателя.
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
