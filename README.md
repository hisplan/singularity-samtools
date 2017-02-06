# singularity-samtools

Singularity for samtools

## Prerequisites

- Singularity 2.2 must be installed on your system. [Here](http://singularity.lbl.gov/docs-quick-start-installation) is the instruction. 

## Build

Download `Singularity` file from this git repository.

Create a 20MB empty image with:

```bash
$ sudo singularity create -s 200 samtools.img
```

Bootstrap the image using the `Singularity` image definition file you downloaded from the previous step:

```bash
$ sudo singularity bootstrap samtools.img Singularity
```

## Run

```bash
$ singularity run samtools.img --help
```

## Notes

- This uses Alpine Linux as base image.
