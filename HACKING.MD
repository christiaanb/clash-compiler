Download sources:
```
git clone git@github.com:clash-lang/clash-compiler.git
git clone git@github.com:clash-lang/clash-prelude.git
```

Go to clash-compiler dir:
```
cd clash-compiler
```

Run:
```
cabal sandbox init
cabal sandbox add-source clash-lib
cabal sandbox add-soruce clash-vhdl
cabal sandbox add-source clash-systemverilog
cabal sandbox add-source clash-ghc
cabal sandbox add-source ../clash-prelude
cabal install clash-ghc --dependencies-only
```

Then to work interactively with the CLaSH compiler, run:
```
./clash-dev
```
