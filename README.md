# CVE-2021-3156 PoC

## Introduction

This is an exploit for the `CVE-2021-3156` sudo vulnerability (dubbed [Baron Samedit](https://www.qualys.com/2021/01/26/cve-2021-3156/baron-samedit-heap-based-overflow-sudo.txt) by Qualys).

## Usage

build:
```
$ make
```

list targets:
```
$ ./sudo-hax-me-a-sandwich
```

run:
```
$ ./sudo-hax-me-a-sandwich <target_number>
```

## Contributing

Send (sensible) PR's, I might merge.

Some ideas:
* More targets
* Target finding
* Other exploitation strategies
* More self contained functionality:
    * Embed shared library hax.c (Make it small please, ELF golf + asm setuid/execve stub)
    * Add mkdir logic to hax.c
* Directory/shared library cleanup
