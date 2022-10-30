First, 
to create the virtual env

    python -m venv cairo_venv

then install cairo

    CFLAGS=-I`brew --prefix gmp`/include LDFLAGS=-L`brew --prefix gmp`/lib pip3 install ecdsa fastecdsa sympy
    pip3 install cairo-lang
