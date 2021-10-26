# hw2 - Оптимизировать код, используя паттерн Worker Pool. Какой прирост в скорости? Почему?

countUsers := 100

workerCount=1	DONE! Time Elapsed: 100.61 seconds
workerCount=2	DONE! Time Elapsed: 50.51 seconds	(в 1,99 раза быстрее)
workerCount=5	DONE! Time Elapsed: 20.53 seconds	(в 4,9 раз быстрее)
workerCount=10	DONE! Time Elapsed: 10.98 seconds	(в 9.16 раз быстрее)
workerCount=100 DONE! Time Elapsed: 10.93 seconds   (в 9.2 раз быстрее)

#Прирост в скорости получается за счет параллельной обработки задачи каждым воркером в отдельной GO рутине
#C определенного момента прирост в скорости не пропорциональный, workers успевают отработать и брать новую работу. 




