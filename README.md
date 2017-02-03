# singularity-samtools

Singularity for samtools

## Build

```bash
$ sudo singularity create -s 200 samtools.img
$ sudo singularity bootstrap samtools.img Singularity
```

## Run

```bash
$ singularity run samtools.img --help
```

## Notes

- This uses Alpine Linux as base image.
