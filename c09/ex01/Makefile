SRCS = ./srcs/ft_putchar.c \
	   ./srcs/ft_swap.c \
	   ./srcs/ft_putstr.c \
	   ./srcs/ft_strlen.c \
	   ./srcs/ft_strcmp.c

HEADERS = ./includes/

OBJS = ${SRCS:.c=.o}

NAME = libft.a

CC = gcc
CFLAGS = -I ${HEADERS} -Wall -Wextra -Werror

.c.o:
	${CC} ${CFLAGS} -c $< -o ${<:.c=.o}

$(NAME): ${OBJS}
	ar rc ${NAME} ${OBJS}

all : ${NAME}

clean:
	rm -f ${OBJS}

fclean: clean
	rm -f ${NAME}

re : fclean all

.PHONY: all clean fclean re
