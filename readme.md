# Basics to run Cairo

First, 
to create the virtual env

    python -m venv cairo_venv

and source it using

    source cairo_venv/bin/activate

then install cairo (this flags are for Apple Sillicon)

    CFLAGS=-I`brew --prefix gmp`/include LDFLAGS=-L`brew --prefix gmp`/lib pip3 install ecdsa fastecdsa sympy
    pip3 install cairo-lang
