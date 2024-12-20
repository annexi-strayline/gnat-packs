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
6.  **gnat-X-gnatcoll\_db.tar.xz**
    Contains AdaCore's gnatcoll-db libraries for sql, sqlite, and xref
7.  **gnat-X-gdb.tar.xz**
    Contains a complementary build of GDB
8.  **gnat-X-elpa_ada_mode.tar.xz**
    Contains a build of the Emacs ELPA Ada Mode binaries
9.   **gnat-X-src.tar.xz**
    Contains the full source collection used to build the packages

These packages are fully self-contained, and do not have any other package dependencies

Eventually, these packages will be added to appropriate package repositories.

## x86\_64 FreeBSD

### Builds

1.  GCC-12.3.0 (FreeBSD 14.0-RELEASE)

    -   [gnat-12.3.0-base.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd14.0/gnat-12.3.0-base.tar.xz)
    -   [gnat-12.3.0-xmlada.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd14.0/gnat-12.3.0-xmlada.tar.xz)
    -   [gnat-12.3.0-gpr.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd14.0/gnat-12.3.0-gpr.tar.xz)
    -   [gnat-12.3.0-gnatcoll\_core.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd14.0/gnat-12.3.0-gnatcoll_core.tar.xz)
    -   [gnat-12.3.0-gnatcoll\_iconv.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd14.0/gnat-12.3.0-gnatcoll_iconv.tar.xz)
    -   [gnat-12.3.0-gnatcoll\_xref.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd14.0/gnat-12.3.0-gnatcoll_xref.tar.xz)
    -   [gnat-12.3.0-gnatcoll\_sql.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd14.0/gnat-12.3.0-gnatcoll_sql.tar.xz)
    -   [gnat-12.3.0-gnatcoll\_sqlite.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd14.0/gnat-12.3.0-gnatcoll_sqlite.tar.xz)
    -   [gnat-12.3.0-elpa_ada_mode.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd14.0/gnat-12.3.0-elpa_ada_mode.tar.xz)
    -   [gnat-12.3.0-gdb.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd14.0/gnat-12.3.0-gdb.tar.xz)
    -   [gnat-12.3.0-src.tar.xz](https://gnat-packs.annexi-strayline.com/x86_64-fsf-freebsd14.0/gnat-12.3.0-src.tar.xz)


### Installation

1.  (For each package in order above)
    1.  Verify gpg from the related signatures in this repository

        ```
        $ gpg --import pubkey.asc
        $ gpg --verify gnat-X-y.tar.xz.sig gnat-X-y.tar.xz
        ```
    
    2.  Extract the package as root
        
        ```# tar zxPf gnat-X-y.tar.xz```

2.  Modify ~/.profile or equivalent:

    ```
    export PATH=/usr/local/gcc-fsf-gnat/bin:$PATH
    export LD_LIBRARY_PATH=/usr/local/gcc-fsf-gnat/lib:/usr/local/gcc-fsf-gnat/lib/gcc/x86_64-fsf-freebsd13.0/10.3.0/adalib:$LD_LIBRARY_PATH
    ```

    Optionally you may want to set LD_RUN_PATH to the same value as LD_LIBRARY_PATH to ensure that executables built with the compiler do not require the same library path to be specified when run.

    For cases where the Ada runtime is to be linked dynamically, you will also need to add the path to the Ada runtime to LD_LIBRARY_PATH (and optionally LD_RUN_PATH). That path can be provided by GCC directly:
    ```
    export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$(gcc --print-file-name adalib)
    ```

## MacOS

### Builds

1.  GCC-14.2.0 (aarch64 MacOS Sequoia 15.1/Darwin 24.1.0)

    -   [gnat-14.2.0-base.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin24.1.0/gnat-14.2.0-base.tar.bz2)
    -   [gnat-14.2.0-xmlada.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin24.1.0/gnat-14.2.0-xmlada.tar.bz2)
    -   [gnat-14.2.0-gpr.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin24.1.0/gnat-14.2.0-gpr.tar.bz2)
    -   [gnat-14.2.0-gnatcoll\_core.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin24.1.0/gnat-14.2.0-gnatcoll_core.tar.bz2)
    -   [gnat-14.2.0-gnatcoll\_iconv.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin24.1.0/gnat-14.2.0-gnatcoll_iconv.tar.bz2)
    -   [gnat-14.2.0-gnatcoll\_db.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin24.1.0/gnat-14.2.0-gnatcoll_db.tar.bz2)
    -   [gnat-14.2.0-elpa_ada_mode.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin24.1.0/gnat-14.2.0-elpa_ada_mode.tar.bz2)
    -   [gnat-14.2.0-src.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin24.1.0/gnat-14.2.0-src.tar.bz2)

2.  GCC-12.3.0 (aarch64 MacOS Sonoma 14.2.1/Darwin 23.2.0)

    -   [gnat-12.3.0-base.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin23.2.0/gnat-12.3.0-base.tar.bz2)
    -   [gnat-12.3.0-xmlada.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin23.2.0/gnat-12.3.0-xmlada.tar.bz2)
    -   [gnat-12.3.0-gpr.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin23.2.0/gnat-12.3.0-gpr.tar.bz2)
    -   [gnat-12.3.0-gnatcoll\_core.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin23.2.0/gnat-12.3.0-gnatcoll_core.tar.bz2)
    -   [gnat-12.3.0-gnatcoll\_iconv.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin23.2.0/gnat-12.3.0-gnatcoll_iconv.tar.bz2)
    -   [gnat-12.3.0-gnatcoll\_xref.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin23.2.0/gnat-12.3.0-gnatcoll_xref.tar.bz2)
    -   [gnat-12.3.0-gnatcoll\_sql.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin23.2.0/gnat-12.3.0-gnatcoll_sql.tar.bz2)
    -   [gnat-12.3.0-gnatcoll\_sqlite.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin23.2.0/gnat-12.3.0-gnatcoll_sqlite.tar.bz2)
    -   [gnat-12.3.0-elpa_ada_mode.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin23.2.0/gnat-12.3.0-elpa_ada_mode.tar.bz2)
    -   [gnat-12.3.0-src.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin23.2.0/gnat-12.3.0-src.tar.bz2)

3.  GCC-11.3.0 (aarch64 MacOS Ventura 13.4/Darwin 22.5.0)

    -   [gnat-11.3.0-base.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin22.5.0/gnat-11.3.0-base.tar.bz2)
    -   [gnat-11.3.0-xmlada.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin22.5.0/gnat-11.3.0-xmlada.tar.bz2)
    -   [gnat-11.3.0-gpr.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin22.5.0/gnat-11.3.0-gpr.tar.bz2)
    -   [gnat-11.3.0-gnatcoll\_core.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin22.5.0/gnat-11.3.0-gnatcoll_core.tar.bz2)
    -   [gnat-11.3.0-gnatcoll\_iconv.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin22.5.0/gnat-11.3.0-gnatcoll_iconv.tar.bz2)
    -   [gnat-11.3.0-gnatcoll\_xref.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin22.5.0/gnat-11.3.0-gnatcoll_xref.tar.bz2)
    -   [gnat-11.3.0-gnatcoll\_sql.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin22.5.0/gnat-11.3.0-gnatcoll_sql.tar.bz2)
    -   [gnat-11.3.0-gnatcoll\_sqlite.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin22.5.0/gnat-11.3.0-gnatcoll_sqlite.tar.bz2)
    -   [gnat-11.3.0-elpa_ada_mode.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin22.5.0/gnat-11.3.0-elpa_ada_mode.tar.bz2)
    -   [gnat-11.3.0-src.tar.bz2](https://gnat-packs.annexi-strayline.com/aarch64-apple-darwin22.5.0/gnat-11.3.0-src.tar.bz2)

4.  GCC-11.3.0 (x86_64 MacOS/Darwin 21.6.0)

    -   [gnat-11.3.0-base.tar.bz2](https://gnat-packs.annexi-strayline.com/x86_64-apple-darwin21.6.0/gnat-11.3.0-base.tar.bz2)
    -   [gnat-11.3.0-xmlada.tar.bz2](https://gnat-packs.annexi-strayline.com/x86_64-apple-darwin21.6.0/gnat-11.3.0-xmlada.tar.bz2)
    -   [gnat-11.3.0-gpr.tar.bz2](https://gnat-packs.annexi-strayline.com/x86_64-apple-darwin21.6.0/gnat-11.3.0-gpr.tar.bz2)
    -   [gnat-11.3.0-gnatcoll\_core.tar.bz2](https://gnat-packs.annexi-strayline.com/x86_64-apple-darwin21.6.0/gnat-11.3.0-gnatcoll_core.tar.bz2)
    -   [gnat-11.3.0-gnatcoll\_iconv.tar.bz2](https://gnat-packs.annexi-strayline.com/x86_64-apple-darwin21.6.0/gnat-11.3.0-gnatcoll_iconv.tar.bz2)
    -   [gnat-11.3.0-gnatcoll\_xref.tar.bz2](https://gnat-packs.annexi-strayline.com/x86_64-apple-darwin21.6.0/gnat-11.3.0-gnatcoll_xref.tar.bz2)
    -   [gnat-11.3.0-gnatcoll\_sql.tar.bz2](https://gnat-packs.annexi-strayline.com/x86_64-apple-darwin21.6.0/gnat-11.3.0-gnatcoll_sql.tar.bz2)
    -   [gnat-11.3.0-gnatcoll\_sqlite.tar.bz2](https://gnat-packs.annexi-strayline.com/x86_64-apple-darwin21.6.0/gnat-11.3.0-gnatcoll_sqlite.tar.bz2)
    -   [gnat-11.3.0-elpa_ada_mode.tar.bz2](https://gnat-packs.annexi-strayline.com/x86_64-apple-darwin21.6.0/gnat-11.3.0-elpa_ada_mode.tar.bz2)
    -   [gnat-11.3.0-gdb.tar.bz2](https://gnat-packs.annexi-strayline.com/x86_64-apple-darwin21.6.0/gnat-11.3.0-gdb.tar.bz2)
    -   [gnat-11.3.0-src.tar.bz2](https://gnat-packs.annexi-strayline.com/x86_64-apple-darwin21.6.0/gnat-11.3.0-src.tar.bz2)


### Installation

1.  (For each package in order above)
    1.  Verify gpg from the related signatures in this repository

        ```
        $ gpg --import pubkey.asc
        $ gpg --verify gnat-X-y.tar.bz2.sig gnat-X-y.tar.bz2
        ```
    
    2.  Extract the package as root
        
        ```# tar zxPf gnat-X-y.tar.bz2```

2.  Modify ~/.profile or equivalent:
    
    

    ### For Apple Silicon (aarch64)
    Apple silicon builds have moved to use '/opt' as the root.
     ```
    export PATH=/usr/local/gcc-fsf-gnat/bin:$PATH
    export DYLD_LIBRARY_PATH=/opt/gcc-fsf-gnat/lib:$DYLD_LIBRARY_PATH
    ```
    ### For x86
    ```
    export PATH=/usr/local/gcc-fsf-gnat/bin:$PATH
    export DYLD_LIBRARY_PATH=/usr/local/gcc-fsf-gnat/lib:$DYLD_LIBRARY_PATH
    ```

    For cases where the Ada runtime is to be linked dynamically, you will also need to add the path to the Ada runtime to DYLD_LIBRARY_PATH (and optionally LD_RUN_PATH). That path can be provided by GCC directly:
    ```
    export DYLD_LIBRARY_PATH=$DYLD_LIBRARY_PATH:$(gcc --print-file-name adalib)
    ```