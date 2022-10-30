# Basics to run Cairo

First, 
to create the virtual env

    python -m venv cairo_venv

and source it using

    source cairo_venv/bin/activate

then install cairo (this flags are for Apple Sillicon)

    CFLAGS=-I`brew --prefix gmp`/include LDFLAGS=-L`brew --prefix gmp`/lib pip3 install ecdsa fastecdsa sympy
    pip3 install cairo-lang

running the code

    cairo-compile new.cairo --output new_compiled.json

    cairo-run --program=new_compiled.json \
    --print_output --layout=small --program_input=puzzle_input.json