#### `nogil`[](https://numba.pydata.org/numba-doc/latest/user/jit.html#nogil "Permalink to this headline")

Whenever Numba optimizes Python code to native code that only works on native types and variables (rather than Python objects), it is not necessary anymore to hold Python’s [global interpreter lock](https://docs.python.org/3/glossary.html#term-global-interpreter-lock "(in Python v3.8)") (GIL). Numba will release the GIL when entering such a compiled function if you passed `nogil=True`.

@jit(nogil=True)
def f(x, y):
    return x + y

Code running with the GIL released runs concurrently with other threads executing Python or Numba code (either the same compiled function, or another one), allowing you to take advantage of multi-core systems. This will not be possible if the function is compiled in [object mode](https://numba.pydata.org/numba-doc/latest/glossary.html#term-object-mode).

When using `nogil=True`, you’ll have to be wary of the usual pitfalls of **multi-threaded programming** (consistency, synchronization, race conditions, etc.).
