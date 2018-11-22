# Описание интерфейса ITeacher
Интерфейс предназначен для работы с методами класса Teacher

## Реализация интерфейса
* +AddTeacher (Teacher:[Person](https://github.com/polinanch/Documents/blob/master/Person.md "объект класса Person")): Int — функция, добавляющая преподавателя в базу данных. Параметр
 «Teacher» — преподаватель, 
которого необходимо добавить в БД;
* +EdiTeacher (Teacher:[Person](https://github.com/polinanch/Documents/blob/master/Person.md "объект класса Person")): Bool — функция, редактирующая
 данные о преподавателе. Параметр «Teacher:Teacher» — 
преподаватель, которого необходимо редактировать в БД;
* +FindByID(ID: Int): Teacher  — функция, осуществляющая 
поиск преподавателя в базе данных по ID и возвращающая найденный, если такой есть. 
* +Del(ID): Bool – функция удаляет преподавателя.
* +Getchedule(ID : int) : List<[Schedule](https://github.com/polinanch/Documents/blob/master/Schedule.md)> - функция возвращающая расписание преподавателя.
* +GetAllCourses(ID : int) : List<[Courses](https://github.com/polinanch/Documents/blob/master/Course.md)> - функция возвращает список курсов данного преподавателя.
* +GetAllGroup(ID : int) : List<[Groups](https://github.com/polinanch/Documents/blob/master/Group.md)> - функция возвращает список групп данного преподавателя.
* +GetAllLanguage(ID : int) :  List<[Languages](https://github.com/polinanch/Documents/blob/master/Language.md)> - функция возвращает список изучаемых языков данного преподавателя.
* +GetAllSalary (ID : int) : List<[Salary](https://github.com/polinanch/Documents/blob/master/Salary.md)> - функция возвращает список зарплат преподавателя.
* +GetAllTeachers(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Person](https://github.com/polinanch/Documents/blob/master/Person.md "объект класса Person")> — функция, возвращающая список преподавателей. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
