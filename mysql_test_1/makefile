CC=gcc
#MYSQLCFLAGS=-I/usr/local/Cellar/mysql/5.6.15/include/mysql -Os -g -fno-strict-aliasing
#MYSQLLIBS=-L/usr/local/Cellar/mysql/5.6.15/lib -lmysqlclient
#INCLUDES=/usr/local/Cellar/mysql/5.6.15/include/mysql/mysql.h
#CFLAGS = $(shell mysql_config --cflags) $(shell mysql_config --libs)

test_1_make: test_1.c
	$(CC) -o test_1 $(shell mysql_config --cflags) test_1.c $(shell mysql_config --libs)
clean:
	rm -f test_1