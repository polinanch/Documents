# Описание интерфейса ISchedule
Интерфейс предназначен для работы с методами класса Schedule

## Реализация интерфейса
* +AddSchedule (Schedule:[Schedule](https://github.com/polinanch/Documents/blob/master/Schedule.md "объект класса Schedule")): Int — функция, добавляющая расписание в базу данных. Параметр «[Schedules](ссылка "объект класса Schedules")» — расписание, 
которое необходимо добавить в БД;
* +EditSchedule (Schedule:[Schedule](https://github.com/polinanch/Documents/blob/master/Schedule.md "объект класса Schedule")): Bool — функция, редактирующая данные о расписании. Параметр «Schedules:[Schedules](https://github.com/gogganesko/Orho/blob/master/docs/Schedules.md "объект класса Schedule")» — 
расписание, которое необходимо редактировать в БД;
* +FindByID(ID: Int): [Schedule](https://github.com/polinanch/Documents/blob/master/Schedule.md "объект класса Schedule")  — функция, осуществляющая поиск клиента в базе данных по ID и возвращающая найденный, если такой есть. 
* +Del(ID): Bool – функция удаляет расписание.
* +GetAllSchedules(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Schedule](https://github.com/polinanch/Documents/blob/master/Schedule.md "объект класса Schedule")> — функция, возвращающая список расписаний. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
