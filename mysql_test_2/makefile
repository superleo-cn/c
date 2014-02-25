CC=gcc
#MYSQLCFLAGS=-I/usr/local/Cellar/mysql/5.6.15/include/mysql -Os -g -fno-strict-aliasing
#MYSQLLIBS=-L/usr/local/Cellar/mysql/5.6.15/lib -lmysqlclient
#INCLUDES=/usr/local/Cellar/mysql/5.6.15/include/mysql/mysql.h
#CFLAGS = $(shell mysql_config --cflags) $(shell mysql_config --libs)
#DEPS = test_1.h
#OBJ = test_1.o main_myql.o

main: test_1.o main_mysql.o
	$(CC) test_1.o main_mysql.o -o main_mysql $(shell mysql_config --cflags) $(shell mysql_config --libs)
main_mysql.o: main_mysql.c 
	$(CC) -o main_mysql.o $(shell mysql_config --cflags) -c main_mysql.c 
test_1.o: test_1.c 
	$(CC) -o test_1.o $(shell mysql_config --cflags) -c test_1.c
clean:
	rm -f test_1.o main_myql.o