# Makefile — Atividade 6
# Complete as regras conforme as instruções da ficha.
# ATENÇÃO: os comandos de cada regra devem começar com TAB (não espaços).
# ─────────────────────────────────────────────────────

CC = gcc
CFLAGS = -Wall -g

soma: soma.o
	$(CC) soma.o -o soma
soma: soma.o
	$(CC) soma.o -o soma
soma.o: soma.c
	$(CC) $(CFLAGS) -c soma.c -o soma.o
soma.o: soma.s
	$(CC) -c soma.s -o soma.o
clean:
	rm -f soma soma.o soma.i soma.s
soma.s: soma.i
	$(CC) -S soma.i -o soma.s
.PHONY: clean
Makefile
CC = gcc
CFLAGS = -Wall -g
soma.i: soma.c
	$(CC) -E soma.c -o soma.i
clean:
	rm -f soma soma.o soma.i soma.s
