all: tsp

CXX=mpic++
CXXFLAGS=-O3 -std=c++0x
CXXFLAGS_DEBUG= -std=c++0x -g
LDFLAGS=-lpthread -lmpi -lmpi_cxx

tsp: tsp.cpp
	$(CXX) $(CXXFLAGS) $(LDFLAGS) $^ -o $@

debug: tsp.cpp
	$(CXX) $(CXXFLAGS_DEBUG) $(LDFLAGS) $^ -o $@

clean:
	rm tsp 

run280:
	mpirun -np 4 ./tsp ../../benchmark/a280.tsp

run100:
	mpirun -np 4 ./tsp ../../benchmark/kroA100.tsp

run38:
	mpirun -np 4 ./tsp ../../benchmark/Djibouti_38.txt

run734:
	mpirun -np 4 ./tsp ../../benchmark/Uruguay_734.txt

run100_8:
	mpirun -np 8 ./tsp ../../benchmark/kroA100.tsp

run493:
	mpirun -np 4 ./tsp ../../benchmark/d493.tsp

run194:
	mpirun -np 4 ./tsp ../../benchmark/Qatar_194.txt

run1979:
	mpirun -np 4 ./tsp ../../benchmark/Oman_1979.txt

run493_8:
	mpirun -np 8 ./tsp ../../benchmark/d493.tsp

run1291:
	mpirun -np 4 ./tsp ../../benchmark/d1291.tsp

runoman:
	mpirun -np 4 ./tsp ../../benchmark/Oman_1979.txt

run3400:
	mpirun -np 4 ./tsp ../../benchmark/Nicaragua_3496.txt
