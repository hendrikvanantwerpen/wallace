#*********************************************************************************************************************#
#                                                                                                                     #
#                                                    Wallace                                                          #
#                                                                                                                     #
#                               Fran�ois Pottier, projet Cristal, INRIA Rocquencourt                                  #
#                                                                                                                     #
#    Copyright 2000 Institut National de Recherche en Informatique et Automatique. Distributed only by permission.    #
#                                                                                                                     #
#*********************************************************************************************************************#
# This pseudo-makefile builds Gromit and Wallace before transferring
# control to the actual makefile.

all:
	@(cd ../gromit; make)
	@(cd ../wallace; make)
	@make -f Makefile.local

depend:
	@(cd ../gromit; make depend; make)
	@(cd ../wallace; make depend)
	@make -f Makefile.local depend

clean:
	@make -f Makefile.local clean

realclean:
	@(cd ../gromit; make clean)
	@(cd ../wallace; make clean)
	@make -f Makefile.local clean

doc:
	@make -f Makefile.local doc

