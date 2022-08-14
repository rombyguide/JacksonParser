# Парсер Московского метрополитена  
## Программа, которая:
- Получает HTML-код страницы Московского метрополитена» с помощью библиотеки jsoup.
- Парсит полученную страницу и получает из неё: 
  - линии московского метро (имя и номер линии, цвет не нужен);
  - станции московского метро (имя станции и номер линии).
- Собирает данные о станциях метро — даты их открытия и глубину станций — из файлов формата CSV и JSON, обходя папки, лежащие в архиве. Разархивируйте архив и напишите код, который будет обходить все вложенные папки, искать в папках файлы JSON и CSV и обрабатывать их в зависимости от формата. Метод для обхода папок должен принимать путь до папки в которой надо производить поиск.
- Создаёт и записывает на диск два JSON-файла:
  - Файл со списком станций по линиям и списком линий по формату JSON-файла (файл map.json)
  - Файл stations.json со свойствами станций {name, line, date, depth, hasConnection}.
