CXX   = g++
CXXFLAGS = -Wall -std=c++11
MAIN     = main
_MAIN    = ${MAIN:%=%.cc}
SRCS     = request gui bank exponential
_SRCS    = ${SRCS:%=%.cc}
_OBJS    = ${SRCS:%=%.o}
TRGT     = main
LNKFLGS  = -pthread

all:
	$(CXX) $(CXXFLAGS) -c $(_SRCS)
	$(CXX) $(CXXFLAGS) -o $(TRGT) $(_MAIN) $(_OBJS) $(LNKFLGS)
clean:
	rm $(TRGT) $(_OBJS)
