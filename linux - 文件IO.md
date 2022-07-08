### 1.buffered i/o and unbuffered i/o

in linux,everything is a file.
for ordinary files,use buffered i/o function to accelerate access.
for device files,use unbuffered i/o function to avoid device waiting.

### 2.unbuffered i/o function:

in unix,<unistd.h> --- read/write
in windows,win32 api --- ReadFile,WriteFile

### 3.其他重要的io函数

open/close	read/write	lseek	fcntl	ioctl	mmap