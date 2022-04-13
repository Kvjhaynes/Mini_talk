FLAGS = -Wall -Werror -Wextra
CC = gcc

SERVER = server
CLIENT = client

PRINTF = ft_printf
FLAGS = -Wall -Wextra -Werror -I$(PRINTF)/ -L$(PRINTF) -lftprintf

all:
		@make -s -C $(PRINTF)
		@gcc $(FLAGS) server.c -o $(SERVER)
		@gcc $(FLAGS) client.c -o $(CLIENT)
		@echo "[SERVER AND CLIENT SUCCESSFULLY CREATED]"

clean:
		@make clean -s -C $(PRINTF)

fclean: clean
		@make fclean -s -C $(PRINTF) 
		@rm -f $(SERVER) $(CLIENT)
		@echo "[SERVER AND CLIENT CLEANED SUCCESSFULLY]"

re: fclean all

