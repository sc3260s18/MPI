CC=mpicc
CFLAGS=-Wall -cc=icc
SRC=mpi_trap.c
EXE=mpi_trap

release : $(SRC)
	$(CC) -o $(EXE) $< $(CFLAGS)

.PHONY: clean

clean:
	rm -f $(EXE)