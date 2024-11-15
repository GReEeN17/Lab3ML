# Линейные методы для бинарной классификации

## Набор данных
1. **Выбор набора данных:**  
   Используйте любой набор данных для задачи бинарной классификации. Желательно использовать данные из предыдущей лабораторной работы. Если исходный набор данных предназначен для многоклассовой классификации, объедините несколько классов для преобразования задачи в бинарную классификацию.

2. **Подготовка данных:**  
   - Преобразуйте данные в числовой формат.
   - Нормализуйте данные.
   - Разбейте данные на тренировочную и тестовую части.

3. **Целевая функция:**  
   Определите целевую функцию ошибки или качества для задачи бинарной классификации.

---

## Алгоритмы

### 1. Линейная регрессия с гребневой регуляризацией
- Реализуйте алгоритм линейной регрессии в матричном виде.
- Используйте гребневую регуляризацию.
- Преобразуйте линейную регрессию в алгоритм линейной классификации, заменив целевой признак на ±1.

### 2. Линейная классификация с градиентным спуском
- Реализуйте алгоритм линейной классификации с градиентным спуском.
- Поддерживаемые функции:
  - **Не менее трёх эмпирических рисков** (основанных на вычислении отступа).
  - **Elastic Net регуляризация.**
- Добавьте возможность настройки скорости градиентного спуска.
- Производные и градиенты должны быть рассчитаны аналитически.

### 3. Метод опорных векторов (SVM)
- Реализуйте SVM через:
  - **SMO** или
  - **Градиентный спуск с восстановлением условий.**
- Поддерживайте работу не менее чем с тремя различными ядрами.

---

## Задачи

### 1. Сравнение сложности алгоритмов
- Выберите число итераций для линейной классификации и метода опорных векторов, чтобы оба алгоритма выполняли асимптотически равное число операций.

### 2. Настройка гиперпараметров
- Подберите лучшие гиперпараметры для каждого алгоритма.

### 3. Анализ обучения
- Постройте **кривую обучения** со сглаженным эмпирическим риском на тренировочном множестве для:
  - Линейной классификации.
  - Метода опорных векторов.

### 4. Тестирование на тестовом множестве
- Постройте **кривую обучения** с целевой функцией ошибки или качества на тестовом множестве:
  - Для линейной классификации.
  - Для метода опорных векторов.
- Замечания:
  - Если итераций много, можно замерять целевую функцию не на каждой итерации.
  - Проведите эксперименты с разными разбиениями на тренировочную и тестовую части.
  - Отметьте доверительный интервал на графике.

### 5. Сравнение с линейной регрессией
- На графике тестового множества добавьте значение целевой функции для линейной регрессии в виде горизонтальной линии.

---

## Результаты
- Приведите графики и результаты анализа.
- Опишите поведение каждого алгоритма и обоснование выбора гиперпараметров.
- Сделайте выводы по качеству и эффективности каждого подхода.