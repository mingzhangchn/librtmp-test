

SRC=librtmp_send264.cpp simplest_librtmp_send264.cpp
OBJ=librtmp_send264.o simplest_librtmp_send264.o

APP=test


INCLUDES = -I./ -I../include

.PONEY:all

all:$(APP) 


$(APP):$(OBJ) 
	@g++  $(OBJ) ../lib/librtmp.a ../lib/libssl.a ../lib/libcrypto.a -ldl -lm -lz -o $@ 

    
%.o:%.cpp
	g++ -c  -fPIC $(INCLUDES) $< -o $@
	
%.o:%.c
	gcc -c $(INCLUDES) $< -o $@    
    
clean:
	@rm -rf $(OBJ) $(APP)
	
	
