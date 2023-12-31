# Palindrom search by FSM

<img src="fsm.png"></img><br>

В данном проекте представлен алгоритм поиска палиндромов в тексте.
Для данного алгоритма была составлена спецификация системы в виде конечного автомата,
а также составлен W-тест с помощью [FSMTest](http://fsmtestonline.ru/).

Данный проект использует [bazel](https://bazel.build/install) в качестве сборщика проекта.
Этот сборщик был выбран для того, чтобы можно было легко применять google-tests к реализации.

## Build (Сборка)

```
cd ~/Algorithms/Palindrom_search/
bazel build //sources:palindrom-search-fsm
```

Сборка в качестве библиотеки - статической и динамической
building for libraries - static and dynamic :
```
bazel build //sources:palindrom_search_fsm_lib
```

## Run (Запуск)

```
cd ~/Algorithms/Palindrom_search/
bazel-bin/sources/palindrom-search-fsm
```
## TEST (Тестирование)
```
cd ~/Algorithms/Palindrom_search/
bazel test --cxxopt=-std=c++17 --test_output=all //tests:palindrom_srch_test 
```
