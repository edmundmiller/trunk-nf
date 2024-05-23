# Toy branch example

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
