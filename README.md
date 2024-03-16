# Hey! I'm Filing Here

In this lab, I successfully implemented a 1 MiB `ext2` file system with 2 directories, 1 regular file, and 1 symbolic link.

## Building

```
make  # compile the executable
```

## Running

```
./ext2-create   # run the executable to create cs111 -base.img
dumpe2fs cs111-base.img  # dumps the filesystem information to help debug
fsck.ext2 cs111-base.img  # this will check that your filesystem is correct
mkdir mnt   # create a directory to mnt your filesystem to
sudo mount -o loop cs111-base.img mnt  # mount your filesystem , loop lets you use a file
ls -ain mnt/  # list all files
```


## Cleaning up

```
sudo umount mnt  # unmount the filesystem when you're done
rmdir mnt  # delete the directory used for mounting when you're done
make clean
```
