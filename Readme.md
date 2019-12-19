User space libraries for ZynqMP with Mali-400
====================================================================================

Overview
------------------------------------------------------------------------------------

### Introduction

This is a repository for making user space libraries debian package for ZynqMP with Mali400.

### Note

This repository only provides script files for creating debian packages. Does not include generated debian package and user space libraries. Download the user space libraries from the Xilinx web page.

Build Debian Package
------------------------------------------------------------------------------------

### Download this repository

```console
shell$ git clone --recursive --depth=1 -b v1.6-2 git://github.com/ikwzm/libmali-zynqmp.git
shell$ cd libmali-zynqmp
```

### Build

```console
shell$ sudo debian/rules binary
```

Download User space libraries(r8p0-01rel0)
------------------------------------------------------------------------------------

### Download with wget

```console
shell$ wget https://www.xilinx.com/publications/products/tools/mali-400-userspace.tar 
--2019-12-08 21:39:58--  https://www.xilinx.com/publications/products/tools/mali-400-userspace.tar
Resolving www.xilinx.com (www.xilinx.com)... 23.32.93.47
Connecting to www.xilinx.com (www.xilinx.com)|23.32.93.47|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 572887040 (546M) [application/x-tar]
Saving to: ‘mali-400-userspace.tar’

mali-400-userspace.tar     100%[=======================================>] 546.35M  21.1MB/s    in 26s     

2019-12-08 21:40:25 (21.0 MB/s) - ‘mali-400-userspace.tar’ saved [572887040/572887040]

```

### Extract mali/rel-v2019.1/r8p0-01rel0.tar to r8p0-01rel0

```console
shell$ tar xf mali-400-userspace.tar mali/rel-v2019.1/r8p0-01rel0.tar
shell$ tar xf mali/rel-v2019.1/r8p0-01rel0.tar
```
