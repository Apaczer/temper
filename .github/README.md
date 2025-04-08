# Temper - NEX/PC-Engine (CD and SuperGrafx) emulator

This is a downstream fork of `Temper` an emu from gp2x aimed here at MiyooCFW (with SDL frontend)

## BIOS

The emulator will recognize BIOSes by placing them in `/$HOME/.temper/syscards/`

## Native build (linux):

- compile & build
```
make -j$(nproc) -C SDL/
```
- run binary from PWD
```
./SDL/temper
```

## Cross-Compile build (MiyooCFW):

It is recommended to use latest toolchain (gcc-9.4.0)

- compile binary (e.g. via docker):
```
make -C SDL/ -f Makefile.miyoo
```
for more optimization (less compatiblity) add `FAST_BUILD=1` flag to make
