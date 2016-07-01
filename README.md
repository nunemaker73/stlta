# STL_TA library

## About this library project
STL_TA began with the need to have an STL compliant Technical Analysis Library. The functions are mostly functor objects that work with other STL algortithms. The functions.cpp is a simple implementation of the actual functor objects into very usable functions.

This library can work entirely with only the header files since the source is primarily for ease of use coinciding with popular Technical Analysis Functions.

Most of the function background was from the following book. There is a big section and each function is very technically described and functions can be derived from the text with relative ease. Future versions of this Library should use either the cited version of the revised edition published in 2014.

	Elder, Alexander. Trading For a Living: Psychology, Trading Tactics, Money Management. New York: John Wiley & Sons, 1992.
	
## 	License
The LICENSE file contains the license this is released under. Contributions to the source code are welcomed.

## Installation
Call the following shell code block:

	libtoolize
	aclocal
	automake --add-missing --gnu
	autoconf
	./configure
	make
	make install
	
You may have to prefix `make install` with a `sudo` command.

## Usage
The library was built with automake tools, and the following instructions apply to using with a program built with the automake tools.

In the Makefile.am add the following line, where prog is the program name variable.

	prog_LDADD=libstlta.la
	

	