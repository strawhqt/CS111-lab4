# Hey! I'm Filing Here

In this lab, I successfully implemented a 1 MiB ext2 file system with 2 directories, 1 regular file, and 1 symbolic link

## Building

```
make
```

## Running

```
./ext2-create
mkdir mnt 
sudo mount -o loop cs111 -base.img mnt
```


## Cleaning up

```
sudo umount mnt
rmdir mnt
make clean
```
