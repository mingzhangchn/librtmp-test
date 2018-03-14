

SRC=simplest_librtmp_sendflv.cpp
OBJ=simplest_librtmp_sendflv.o

APP=test


INCLUDES = -I../include

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
	
	
