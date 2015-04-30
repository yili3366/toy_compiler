DIRS =  \
         compiler \
         debug \
         dvm \
         memory \
         share

CFLAGS = -g3 -gdwarf-4

all:
	@ for dir in ${DIRS}; do (cd $${dir}; ${MAKE}) ; done
clean:
	@ for dir in ${DIRS}; do (cd $${dir}; ${MAKE} clean) ; done
