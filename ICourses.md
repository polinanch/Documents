# Описание интерфейса Course
Интерфейс предназначен для работы с методами класса Course

## Реализация интерфейса
* +AddCourse (Course:[Course](https://github.com/polinanch/Documents/blob/master/Course.md "объект класса Course")): Int — функция, добавляющая 
курс в базу данных. Параметр «[Course](https://github.com/polinanch/Documents/blob/master/Course.md "объект класса Course")» — курс, 
который необходимо добавить в БД;
* +EditCourse (Course:[Course](https://github.com/polinanch/Documents/blob/master/Course.md  "объект класса Course")): Bool — функция, редактирующая
 данные о курсе. Параметр «[Course](https://github.com/polinanch/Documents/blob/master/Course.md  "объект класса Course")» — 
курс, который необходимо редактировать в БД;
* +FindByID(ID: Int): [Course](https://github.com/polinanch/Documents/blob/master/Course.md  "объект класса Course")  — функция, осуществляющая
 поиск курса в базе данных по ID и возвращающая найденный, если такой есть. 
* +Del(ID): Bool – функция удаляет курс.
<[Course](https://github.com/polinanch/Documents/blob/master/Course.md  "объект класса Course")> — функция, возвращающая список курсов. 
* +GetAllStudent(ID : int) List<[Client](https://github.com/polinanch/Documents/blob/master/Client.md )> - функция возвращающая список учащихся на этом курсе.
* +Getchedule(ID : int) List<[Schedule](https://github.com/polinanch/Documents/blob/master/Schedule.md )> - функция возвращающая расписание заданного курса.
* +GetAllCourses(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
