# Проект Калькулятор для работы с полиномами и выражениями

## Содержание проекта
---
Проект демонстрирует парсинг инфиксных выражений в обратную польскую запись (RPN), 
вычисление значений выражений, арифметику над полиномами и дифференцирование.

## Реализованы следующие возможности:

- **Парсинг инфиксных выражений** в обратную польскую запись (RPN).
- **Вычисление выражений** с числами и переменными.
- **Арифметика над полиномами:** сложение, вычитание, умножение.
- **Дифференцирование полиномов** по x, y, z.
- **Структуры данных:** односвязный список, кольцевой список, стек.
- **Юнит-тесты** GoogleTest.
- **Примеры** директория `samples`.

## Структура проекта
```
├── gtest/                          
│   ├── CMakeLists.txt
│   ├── gtest.h
│   └── gtest-all.cc
├── lib_expression/                 
│   ├── include/
│   │   ├── ArExpression.h
│   │   ├── Stack.h
│   │   └── SupFunctions.h
│   └── src/
│       ├── ArExpression.cpp
│       ├── Stack.cpp
│       └── SupFunctions.cpp
├── lib_lists/                      
│   ├── include/
│   │   ├── TList.h
│   │   ├── TNode.h
│   │   └── TRingList.h
│   └── src/
│       ├── TList.cpp
│       ├── TNode.cpp
│       └── TRingList.cpp
├── lib_tpolynoms/                  
│   ├── include/
│   │   ├── TMonom.h
│   │   └── TPolynom.h
│   └── src/
│       ├── TMonom.cpp
│       └── TPolynom.cpp
├── samples/                        
│   ├── sample_TList.cpp
│   ├── sample_TMonom.cpp
│   ├── sample_TNode.cpp
│   └── sample_TPolynom.cpp
├── tests/                          
│   ├── test_TList.cpp
│   ├── test_ArExpression.cpp
│   ├── test_Stack.cpp
│   ├── test_TMonom.cpp
│   ├── test_TNode.cpp
│   ├── test_tpolynoms.cpp
│   └── test_TRingList.cpp               
├── .gitignore
├── CMakeLists.txt
└── README.md
```

## Технологический стек

*   **Язык** C++14 
*   **Система сборки** CMake
*   **Тестирование** GoogleTest
*   **Структуры данных** Односвязный список, кольцевой односвязный список, стек 
*   **Алгоритмы** RPN, парсинг, полиномы 

## Требования к системе

- **Компилятор с поддержкой C++14:**
  - GCC 5+
  - Clang 3.4+
  - MSVC 2015+ (Visual Studio 2015 или новее)
- **CMake** 3.7+

---

## Сборка проекта

1.  **Клонирование репозитория:**
    ```bash
    git clone https://github.com/Kirius257/Calculator.git
    cd Calculator
    ```

2.  **Создание системы сборки:**
    ```bash
    mkdir build && cd build
    cmake ..
     ```

3.  **Сборка проекта:**
    ```bash
    cmake --build build --config Release
    ```

4.  **Запуск тестов:**
    ```bash
    cd build/bin/
    <имя исполняемого файла для теста>
    ```
     Используйте табуляцию для выбора файла для теста 
---
