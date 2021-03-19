all: buffsize100 buffsize4096 buffsize8192 buffsize16384 buffsize4096_fsync

buffsize100: buffsize100.o error.o
	$(CC) -g -o $@ $^
	
buffsize4096: buffsize4096.o error.o
	$(CC) -g -o $@ $^	

buffsize4096_fsync: buffsize4096_fsync.o error.o
	$(CC) -g -o $@ $^		
	
buffsize8192: buffsize8192.o error.o
	$(CC) -g -o $@ $^	
	
buffsize16384: buffsize16384.o error.o
	$(CC) -g -o $@ $^		
	
buffsize100.o: buffsize100.c 
	$(CC) -g -c buffsize100.c
	
buffsize4096.o: buffsize4096.c 
	$(CC) -g -c buffsize4096.c	

buffsize4096_fsync.o: buffsize4096_fsync.c 
	$(CC) -g -c buffsize4096_fsync.c	
	
buffsize8192.o: buffsize8192.c 
	$(CC) -g -c buffsize8192.c		
	
buffsize16384.o: buffsize16384.c 
	$(CC) -g -c buffsize16384.c	
	
error.o: error.c
	$(CC) -g -c error.c
	
clean:
	rm -f *.o buffsize100 buffsize4096 buffsize8192 buffsize16384 buffsize4096_fsync
