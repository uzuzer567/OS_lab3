# Лабораторная работа №3

Вариант 5.

Реализовать на основе принципов RPC механизм вычисления произвольной математической функции. Разработанная клиент-серверная архитектура на базе RPC должна позволять легкое добавление и удаление новых RPC-процедур. Для упрощения реализации будем считать что RPC-вызов должен осуществляться только из приложений реализованных на языке С++.

Выполнила студентка группы 821703 Стасько Валерия.

# Установка

1. Clone project;
2. Make maths;
3. Run maths;
4. Make server;
5. Make client;

git clone https://github.com/uzuzer567/OS_lab3.git
cd OS_lab3/maths
cmake CMakeLists.txt
make
./maths maths.x
cp maths.h maths_client.cpp ../client
cp maths.h maths_server.cpp ../server
cd ../server
[edit maths_server.cpp if needed]
cmake CMakeLists.txt
make
cd ../client
cmake CMakeLists.txt
make

# Запуск

[console 1]:
cd OS_lab3/server
./server

[console 2]:
cd OS_lab3/client
./client <hostmane>
