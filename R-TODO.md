- 7.3-64 = translate to 7.3.64?
- 

## DONE


MD5 sum is wrong
Dependencies need to go in host as well?
Skip empty python serialization in build.

Are these all from the "default" installation?
- r-stats
- r-graphics
- r-utils
- r-methods
- r-parallel is part of R?


grDevices?


make use of NeedsCompilation: yes/no flags?!

Take into account `sysdeps`, e.g.:

  "_rundeps": [],
  "_sysdeps": [
    {
      "package": "libopenblas0-pthread",
      "source": "openblas",
      "version": "0.3.26+ds-1",
      "name": "openblas",
      "homepage": "https://www.openblas.net/",
      "description": "Optimized BLAS (linear algebra) library (shared lib, pthread)"
    },
    {
      "package": "libopenblas0-pthread",
      "source": "openblas",
      "version": "0.3.26+ds-1",
      "name": "openblas",
      "homepage": "https://www.openblas.net/",
      "description": "Optimized BLAS (linear algebra) library (shared lib, pthread)"
    }
  ],
  "_score": 3.6364878963533656,


Autogenerate tests?!
E.g.

    - $R -e "library('nleqslv')"           # [not win]
    - "\"%R%\" -e \"library('nleqslv')\""  # [win]
