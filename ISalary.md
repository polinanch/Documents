# Описание интерфейса ISalary
Интерфейс предназначен для работы с методами класса Salary

## Реализация интерфейса
* +AddSalary (Salary:[Salary](https://github.com/polinanch/Documents/blob/master/Salary.md "объект класса Salary")): Int — функция, добавляющая 
зарплату в базу данных. Параметр «[Salary](https://github.com/polinanch/Documents/blob/master/Salary.md "объект класса Salarys")» — зарплата, 
которую необходимо добавить в БД;
* +EditSalary (Salary:[Salary](https://github.com/polinanch/Documents/blob/master/Salary.md "объект класса Salary")): Bool — функция, 
редактирующая данные о зарплате. Параметр «Salarys:[Salarys](https://github.com/polinanch/Documents/blob/master/Salary.md "объект класса Salary")» — 
зарплата, которую необходимо редактировать в БД;
* +FindByID(ID: Int): [Salary](https://github.com/polinanch/Documents/blob/master/Salary.md "объект класса Salary")  — функция, осуществляющая поиск 
зарплаты в базе данных по ID и возвращающая найденную, если такая есть. 
* +Del(ID): Bool – функция удаляет зарплату.
* +GetAllSalarys(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Salary](https://github.com/polinanch/Documents/blob/master/Salary.md "объект класса Salary")> — функция, возвращающая список зарплат. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.
