# RollNo : 2018201033  Name : Darshan Kansagara
CC = g++
CFLAGS = -Wall 
DEPS = clientheader.h 
OBJ = share_file.o get_file.o remove_file.o seeder.o torrent_creater.o client.o
%.o: %.cpp $(DEPS)
	$(CC) $(CFLAGS) -c -o $@ $< -lssl -lcrypto -lpthread

client: $(OBJ)
	$(CC) $(CFLAGS) -o $@ $^ -lssl -lcrypto -lpthread

clean:
	rm -rf *o client
