# Hello Cairo with NIX

### Install NIX

**Mac OS**
```shell
sh <(curl -L https://nixos.org/nix/install)
```

**Linux**
```shell
sh <(curl -L https://nixos.org/nix/install) — daemon
```
---

### Let's run Cairo code

**Execute NIX shell**
```shell
nix-shell
```

**Compile code**
```shell
cairo-compile test.cairo --output test_compiled.json
```

**Run code**
```shell
cairo-run --program=test_compiled.json --print_output --print_info --relocate_prints
```
