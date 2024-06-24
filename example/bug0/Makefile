LEVELDB_SRC = /home/jiexiao/squint/alice/alice/example/bug0/leveldb
EXECUTABLES = workload checker init
DEPENDENCIES = common.h Makefile

all: $(EXECUTABLES)

%: %.cc $(LEVELDB_SRC) $(DEPENDENCIES)
	g++ -g -o $@ $< $(LEVELDB_SRC)/build/libleveldb.a -I$(LEVELDB_SRC)/include -lpthread -lsnappy

clean:
	rm -f $(EXECUTABLES)
