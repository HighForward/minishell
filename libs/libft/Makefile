
NAME		=	libft.a

SRCS		=	ft_atoi.c				\
				ft_putchar.c			\
				ft_bzero.c				\
				ft_calloc.c				\
				ft_isalnum.c			\
				ft_isalpha.c			\
				ft_swap.c				\
				ft_isascii.c			\
				ft_isdigit.c			\
				ft_isprint.c			\
				ft_memchr.c				\
				ft_memcmp.c				\
				ft_memcpy.c				\
				ft_memccpy.c			\
				ft_memmove.c			\
				ft_memset.c				\
				ft_strchr.c				\
				ft_strdup.c				\
				ft_strlcat.c			\
				ft_strlcpy.c			\
				ft_strlen.c				\
				ft_strncmp.c			\
				ft_strcmp.c			    \
				ft_strnstr.c			\
				ft_strrchr.c			\
				ft_tolower.c			\
				ft_toupper.c			\
				ft_substr.c				\
				ft_strjoin.c			\
				ft_strtrim.c			\
				ft_split.c				\
				ft_putchar_fd.c			\
				ft_putstr_fd.c			\
				ft_putendl_fd.c			\
				ft_putnbr_fd.c			\
				ft_strmapi.c			\
				ft_itoa.c				\
				ft_strncat.c			\
				ft_strnew.c				\
				ft_putstr.c             \
				ft_strncat.c			\
				ft_strcpy.c				\

BONUS_SRCS =	ft_lstadd_back_bonus.c	\
				ft_lstadd_front_bonus.c	\
				ft_lstclear_bonus.c		\
				ft_lstdelone_bonus.c	\
				ft_lstiter_bonus.c		\
				ft_lstlast_bonus.c		\
				ft_lstmap_bonus.c		\
				ft_lstnew_bonus.c		\
				ft_lstsize_bonus.c		\
				ft_lstrev.c				\


OBJS		=	${SRCS:.c=.o}

BOBJS		=	${BONUS_SRCS:.c=.o}

FLAGS		=	-Wall -Wextra -Werror -g3 -Iincludes

CC			=	gcc

RM			=	rm -f

.c.o:
				@$(CC) $(FLAGS) -c $< -o ${<:.c=.o}
				@printf "\033[2K\033[0;35mLIBFT\033[0;0m:        \033[0;33mCompilation...    \033[0;31m%-15.15s\033[0;0m\r" $(notdir ${<})

$(NAME): ${OBJS}
				@ar rcs $(NAME) ${OBJS}

silent:
			@:

all: $(NAME)

clean:
				@${RM} ${OBJS}
				@${RM} ${BOBJS}

fclean: clean
				@${RM} $(NAME)
				@${RM} ${BOBJS}

re:	fclean all

bonus: $(NAME) $(BOBJS)
				@ar rcs $(NAME) ${BOBJS}

.PHONY: all clean fclean re bonus
