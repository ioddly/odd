CXXFLAGS := -g3 -fno-rtti -fno-exceptions -DPIP_DEBUG
LDFLAGS := 

-include site.mk

all: pip

pip: cli.cpp pip.hpp test/tests.cpp
	@echo -n ' LD  ';
	$(strip $(CXX) $(CPPFLAGS) $(CXXFLAGS) -o $@ $< $(LDFLAGS))

.PHONY: clean cloc update-s7 microgue.c

clean:
	rm -f $(wildcard pip *.o)
