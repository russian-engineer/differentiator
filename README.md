# Differentiator

## Описание проекта

Differentiator изначально задумывался как подспорье перед написанием собственного языка программирования, помогая понять алгоритм рекурсивного спуска. Несмотря на это, проект полезен сам по себе, так как помогает брать производные сложных математических функций.

## Технологии

- **Язык программирования:** C
- **Сборка:** CMake
- **Визуализация дерева выражений:** DOT (Graphviz)
- **Вывод в файл:** LaTeX
- **Unit тесты:** Criterion (в планах)

## Требования и зависимости

- Компилятор C
- CMake
- Graphviz (для визуализации дерева)
- LaTeX (для вывода результата)

## Установка и сборка

1. Клонируйте репозиторий:
    ```sh
    git clone https://github.com/Rustic-soul/Differentiator.git
    cd Differentiator
    ```

2. Создайте директорию для сборки и перейдите в неё:
    ```sh
    mkdir build
    cd build
    ```

3. Сконфигурируйте проект с помощью CMake:
    ```sh
    cmake ..
    ```

4. Соберите проект:
    ```sh
    cmake --build .
    ```

## Использование

1. Поместите математическое выражение, от которого нужно посчитать производную, в файл `path_to_project/images/exp/exp.txt`.

2. Запустите исполняемый файл `differentiator` из папки `path_to_project/build`:
    ```sh
    ./differentiator
    ```

3. Результат будет сохранен в файл `path_to_project/images/tex/res.tex`, который будет содержать исходную функцию и её производную.

4. Вы можете изменить переменную, по которой происходит дифференцирование, в файле `main.c`.

## Планы на будущее

- Добавить тестирование с использованием библиотеки Criterion.
- Дамп промежуточных результатов дифференцирования в файл LaTeX.
- Реализация разложения функции по Тейлору.
- Реализация разложения функции по Маклорену.
- Добавление еще одного алгоритма упрощения получившегося после дифференцирования выражения (помимо свёртки констант и удаления нейтральных элементов).

## Автор

Шляпин Илья

Буду рад обратной связи и предложениям по улучшению проекта!
