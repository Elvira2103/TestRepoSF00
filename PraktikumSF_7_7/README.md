# TestRepoSF00
## Практикум 7_7 SkillFactory
Задание 1
Разработать тест-дизайн и на его основе разработать позитивные API-тесты для тестирования функции фильтрации отбора животных
в веб-приложении «Дом питомца». На выходе должен быть получен файл с вариантами проверок ключей species_name, breed_code, 
gender_code и age. Вы можете использовать разные длины строк и символы. Только помните, что в этом модуле мы разбираем позитивные тесты!
Не нужно писать текстовые символы в числовые поля.
Использовать приложение Postman. Тесты собрать в одну коллекцию. 
Ожидаемый результат — возврат API-запросом кода состояния 200.
Цель — продемонстрировать навыки работы с приложением Postman.

Подходы к решению
В приложении 4 фильтра: пол, порода, вид животного и возраст. В каждом фильтре есть несколько значений, за исключением возраста.

Открыть вкладку Network инструментов разработчика и посмотреть, как передается запрос на отображение списка животных в приложении,
если мы применяем фильтр: какой параметр передается в адресной строке, и какое ему присваивается значение.
Использовать pairwise online tool. Составить таблицу, в которой перечислить все значения каждого параметра. 
Самое главное — не забыть включить пустое значение параметра, когда фильтрация по данному параметру не производится. 
Параметр «возраст» выбрать из диапазона существующих возрастов животных в приложении. 
Далее можно использовать два подхода:
Применить избыточное тестирование. Кликаем на кнопку Generate all combinations, получаем таблицу со всеми комбинациями параметров.
Применить технику pairwise. Кликаем на кнопку Generate pairwise и получаем таблицу со значениями параметров, 
созданными с применением техники pairwise.
Создать запросы в Postman. 
Количество запросов будет равно количеству строк в таблице, полученной с помощью сервиса pairwise online tool. 
Каждая строка таблицы будет содержать параметры для одного запроса.
Добавить в каждый запрос тест на успешное выполнение.
