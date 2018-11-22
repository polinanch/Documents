# Описание интерфейса IRepayment
Интерфейс предназначен для работы с методами класса Repayment

## Реализация интерфейса
* +AddRepayment (Repayment:[Repayment](https://github.com/polinanch/Documents/blob/master/Repayment.md "объект класса Repayment")): Int — 
функция, добавляющая выплату в базу данных. Параметр «[Repayments](https://github.com/polinanch/Documents/blob/master/Repayment.md "объект класса Repayments")» — выплата, 
которую необходимо добавить в БД;
* +EditRepayment (Repayment:[Repayment](https://github.com/polinanch/Documents/blob/master/Repayment.md "объект класса Repayment")): Bool — функция, 
редактирующая данные о выплате. Параметр «Repayments:[Repayments](https://github.com/polinanch/Documents/blob/master/Repayment.md "объект 
класса Repayment")» — 
выплата, которую необходимо редактировать в БД;
* +FindByID(ID: Int): [Repayment](https://github.com/polinanch/Documents/blob/master/Repayment.md "объект класса Repayment")  — функция, осуществляющая поиск 
выплаты в базе данных по ID и возвращающая найденную, если такая есть. 
* +Del(ID): Bool – функция удаляет выплату.
* +GetAllRepayments(ID: Int, sorting: string, sortingA: string, filtering: Reader, count: Int, page: Int): List <[Repayment](https://github.com/polinanch/Documents/blob/master/Repayment.md "объект класса Repayment")> — функция, возвращающая список выплат. 
Параметры: 
	* sortintg: string — отвечает, по какому полю будет сортироваться список;
  
	* sortingA: bool — отвечает, по возрастанию или убыванию будут сортироваться элементы;
  
	* filtering: string — отвечает за фильтрацию;
  
	* count: int — отвечает, сколько элементов необходимо показать;
  
	* page: int — отвечает, с какой страницы начинать поиск элементов.