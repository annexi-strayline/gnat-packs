# gnat-packs - ready-built GCC/GNAT binary packages

Packages are layered in order (package 2 must be installed after
package 1, package 3 after package 2)

1.  **gnat-X-base.tar.xz**
    Contains FSF GCC with C,C++, and Ada, including the full GPL
    runtime exception
2.  **gnat-X-xmlada.tar.xz**
    Contains AdaCore's xmlada library
3.  **gnat-X-gpr.tar.xz**
    Contains AdaCore's gprbuild
4.  **gnat-X-gnatcoll\_core.tar.xz**
    Contains AdaCore's gnatcoll-core libraries
5.  **gnat-X-gnatcoll\_iconv.tar.xz**
    Contains AdaCore's gnatcoll-bindings for iconv
6.  **gnat-X-gnatcoll\_sql.tar.xz**
    Contains AdaCore's gnatcoll-db libraries for sql
7.  **gnat-X-gnatcoll\_sqlite.tar.xz**
    Contains AdaCore's gnatcoll-db libraries for sqlite
8.  **gnat-X-gnatcoll\_xref.tar.xz**
    Contains AdaCore's gnatcoll-db for xref

9.  **gnat-X-gnatcoll\_gdb.tar.xz**
    Contains a complementary build of GDB
10. **gnat-X-elpa_ada_mode.tar.xz**
    Contains a build of the Emacs ELPA Ada Mode binaries
11. **gnat-X-src.tar.xz**
    Contains the full source collection used to build the packages

These packages are fully self-contained, and do not have any other package dependencies

Eventually, these packages will be added to appropriate package repositories.


## x86\_64 Linux

### Builds

1.  GCC-10.3.0

    -   [gnat-10.3.0-base.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.3.0-base.tar.xz)
    -   [gnat-10.3.0-xmlada.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.3.0-xmlada.tar.xz)
    -   [gnat-10.3.0-gprbuild.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.3.0-gpr.tar.xz)
    -   [gnat-10.3.0-gnatcoll\_core.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.3.0-gnatcoll_core.tar.xz)
    -   [gnat-10.3.0-gnatcoll\_iconv.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.3.0-gnatcoll_iconv.tar.xz)
    -   [gnat-10.3.0-gnatcoll\_xref.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.3.0-gnatcoll_xref.tar.xz)
    -   [gnat-10.3.0-gnatcoll\_sql.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.3.0-gnatcoll_sql.tar.xz)
    -   [gnat-10.3.0-gnatcoll\_sqlite.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.3.0-gnatcoll_sqlite.tar.xz)
    -   [gnat-10.3.0-gdb.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.3.0-gdb.tar.xz)
    -   [gnat-10.3.0-elpa_ada_mode.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.3.0-elpa_ada_mode.tar.xz)
    -   [gnat-10.3.0-src.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.3.0-src.tar.xz)

2.  GCC-10.2.0

    -   [gnat-10.2.0-base.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.2.0-base.tar.xz)
    -   [gnat-10.2.0-xmlada.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.2.0-xmlada.tar.xz)
    -   [gnat-10.2.0-gprbuild.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.2.0-gprbuild.tar.xz)
    -   [gnat-10.2.0-gnatcoll\_core.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.2.0-gnatcoll_core.tar.xz)
    -   [gnat-10.2.0-gnatcoll\_iconv.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.2.0-gnatcoll_iconv.tar.xz)
    -   [gnat-10.2.0-gnatcoll\_xref.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.2.0-gnatcoll_xref.tar.xz)
    -   [gnat-10.2.0-gnatcoll\_sql.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.2.0-gnatcoll_sql.tar.xz)
    -   [gnat-10.2.0-gnatcoll\_sqlite.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.2.0-gnatcoll_sqlite.tar.xz)
    -   [gnat-10.2.0-gdb.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.2.0-gdb.tar.xz)
    -   [gnat-10.2.0-src.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-10.2.0-src.tar.xz)

3.  GCC-9.1.0

    -   [gnat-9-base.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-9-base.tar.xz)
    -   [gnat-9-xmlada.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-9-xmlada.tar.xz)
    -   [gnat-9-gprbuild.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-9-gprbuild.tar.xz)
    -   [gnat-9-gnatcoll\_core.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-9-gnatcoll_core.tar.xz)
    -   [gnat-9-src.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-9-src.tar.xz)

4.  GCC-8.3.0

    -   [gnat-8-base.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-8-base.tar.xz)
    -   [gnat-8-xmlada.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-8-xmlada.tar.xz)
    -   [gnat-8-gprbuild.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-8-gprbuild.tar.xz)
    -   [gnat-8-gnatcoll\_core.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-8-gnatcoll_core.tar.xz)
    -   [gnat-8-src.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-linux-gnu/gnat-8-src.tar.xz)

### Installation

1.  (For each package in order above)
    1.  Verify gpg from the related signatures in this repository

        ```
        $ gpg --import pubkey.asc
        $ gpg --verify gnat-X-y.tar.xz.sig gnat-X-y.tar.xz
        ```
    
    2.  Extract the package
        
        ```$ xz -cd gnat-X-y.tar.xz | sudo tar xP```

2.  Modify ~/.bashrc or equivilent:
    ```
    export PATH=/opt/gcc-fsf-gnat/bin:$PATH
    export LD_LIBRARY_PATH=/opt/gcc-fsf-gnat/lib64:/opt/gcc-fsf-gnat/lib
    ```


## x86\_64 FreeBSD

### Builds

1.  GCC-10.3.0 (FreeBSD 13.0-RELEASE)

    -   [gnat-10.3.0-base.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd13.0/gnat-10.3.0-base.tar.xz)
    -   [gnat-10.3.0-xmlada.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd13.0/gnat-10.3.0-xmlada.tar.xz)
    -   [gnat-10.3.0-gpr.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd13.0/gnat-10.3.0-gpr.tar.xz)
    -   [gnat-10.3.0-gnatcoll\_core.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd13.0/gnat-10.3.0-gnatcoll_core.tar.xz)
    -   [gnat-10.3.0-gnatcoll\_iconv.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd13.0/gnat-10.3.0-gnatcoll_iconv.tar.xz)
    -   [gnat-10.3.0-gnatcoll\_xref.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd13.0/gnat-10.3.0-gnatcoll_xref.tar.xz)
    -   [gnat-10.3.0-gnatcoll\_sql.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd13.0/gnat-10.3.0-gnatcoll_sql.tar.xz)
    -   [gnat-10.3.0-gnatcoll\_sqlite.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd13.0/gnat-10.3.0-gnatcoll_sqlite.tar.xz)
    -   [gnat-10.3.0-elpa_ada_mode.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd13.0/gnat-10.3.0-elpa_ada_mode.tar.xz)
    -   [gnat-10.3.0-gdb.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd13.0/gnat-10.3.0-gdb.tar.xz)
    -   [gnat-10.3.0-src.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd13.0/gnat-10.3.0-src.tar.xz)


2.  GCC-10.2.0 (12.2-RELEASE)

    -   [gnat-10.2.0-base.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd12.2/gnat-10.2.0-base.tar.xz)
    -   [gnat-10.2.0-xmlada.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd12.2/gnat-10.2.0-xmlada.tar.xz)
    -   [gnat-10.2.0-gprbuild.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd12.2/gnat-10.2.0-gprbuild.tar.xz)
    -   [gnat-10.2.0-gnatcoll\_core.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd12.2/gnat-10.2.0-gnatcoll_core.tar.xz)
    -   [gnat-10.2.0-gnatcoll\_iconv.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd12.2/gnat-10.2.0-gnatcoll_iconv.tar.xz)
    -   [gnat-10.2.0-gnatcoll\_xref.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd12.2/gnat-10.2.0-gnatcoll_xref.tar.xz)
    -   [gnat-10.2.0-gnatcoll\_sql.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd12.2/gnat-10.2.0-gnatcoll_sql.tar.xz)
    -   [gnat-10.2.0-gnatcoll\_sqlite.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd12.2/gnat-10.2.0-gnatcoll_sqlite.tar.xz)
    -   [gnat-10.2.0-elpa_ada_mode.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd12.2/gnat-10.2.0-elpa_ada_mode.tar.xz)
    -   [gnat-10.2.0-src.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd12.2/gnat-10.2.0-src.tar.xz)


### Installation

1.  (For each package in order above)
    1.  Verify gpg from the related signatures in this repository

        ```
        $ gpg --import pubkey.asc
        $ gpg --verify gnat-X-y.tar.xz.sig gnat-X-y.tar.xz
        ```
    
    2.  Extract the package as root
        
        ```# tar zxPf gnat-X-y.tar.xz```

2.  Modify ~/.profile or equivilent:
    ```
    export PATH=/usr/local/gcc-fsf-gnat/bin:$PATH
    export LD_LIBRARY_PATH=/usr/local/gcc-fsf-gnat/lib:/usr/local/gcc-fsf-gnat/lib/gcc/x86_64-fsf-freebsd13.0/10.3.0/adalib:$LD_LIBRARY_PATH
    ```

