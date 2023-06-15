# simple_shelf_salt_bug

This repo contains configs for MOM6 to run a simple triangular ice shelf. It shows how the salinity initialization with an ice shelf has a bug that isn't 
creating 
linear salinity with repspect to cell depth -- see `Seamount TS.ipynb` for images.

Some further comments:
- The same occurs with a temperature gradient rather than salinity gradient (the default)
- This is not restricted to the chosen `SIGMA_SHELF_ZSTAR` coordinate
- The pattern also occurs with other choices of `TS_CONFIG` and `THICKNESS_CONFIG`.

A hack to fix this is in the branch [`hackfix_v2`](https://github.com/claireyung/simple_shelf_salt_bug/tree/hackfix_v2).
