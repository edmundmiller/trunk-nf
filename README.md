# Toy branch example

```
nextflow run edmundmiller/trunk-nf # -r master
```

## Version in defaultBranch

```nextflow
manifest {
    version         = '1.1.0'
    defaultBranch   = '1.1.0'
    //defaultRevision = ""
}
```

```console
nextflow run edmundmiller/trunk-nf
```

_Fails_ with

```console
Project `edmundmiller/trunk-nf` is currently stuck on revision: master -- you need to explicitly specify a revision with the option `-r` in order to use it
```

## No defaultBranch

```nextflow
manifest {
    version         = '1.1.0'
    // defaultBranch   = '1.1.0'
    //defaultRevision = ""
}
```

Fails with

```console
Project `edmundmiller/trunk-nf` is currently stuck on revision: master -- you need to explicitly specify a revision with the option `-r` in order to use it
```

## defaultBranch = master

Launching `https://github.com/edmundmiller/trunk-nf` [special_lumiere] DSL2 - revision: c9e4ebd02e [master]

executor > local (5)
[b4/b5defe] sayHello (3) [100%] 5 of 5 ✔
Yo world!

Ciao world!

Hola world!

Bonjour world!

Hello world!

## defaultBranch = 1.1.0
