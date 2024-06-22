TARGET = s21_cat
CC = gcc
CFLAGS = -Wall -Wextra -Werror

PREF_OBJ = ./obj/
PREF_SRS = ./SRS/

SRS = $(wildcard *.c)
OBJ = $(patsubst %.c, $(PREF_OBJ)%.o, $(SRS))

$(TARGET): $(OBJ)
	$(CC) $(OBJ) -o $(TARGET)

$(PREF_OBJ)%.o: %.c
	@mkdir -p $(PREF_OBJ)
	$(CC) -c $(CFLAGS) $< -o $@

clean:
	rm -f $(TARGET) $(PREF_OBJ)*.o .clang-format

test:
	bash tests.sh
