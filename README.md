# Motorica_2022
# The task of gesture classification  
Задача классификации жестов  
Команда №5
Состав команды:
- Власов Владимир https://github.com/vip-v2a
- Мархай Ольга
- Плюснин Олег https://github.com/cheef777/SkillFactory
- Ядринцев Алексей https://github.com/Yyalexx

Как можно видеть в представленном ноутбуке мы сначала произвели пороговую фильтрацию сигнала датчиков для устранения шумовой составляющей, затем провели фильтрацию сигнала по медианному или среднему значению окна фильтра. Порог, тип и окно фильтрации задаются в блоке параметров для адаптации под конкретные условия. Предусмотрено удаление нулевых признаков. При формировании новых признаков используются статистические показатели сигнала, а также дифференцирование, шаг дифференцирования задается в блоке параметров.

Подготовка данных для нейронной сети заключалась в пороговой фильтрации и нормализации показаний датчиков по строкам в диапазон значений (0, 1).
Свертка проходила по 60 значениям одного датчика, т.е. не по шкале времени.
