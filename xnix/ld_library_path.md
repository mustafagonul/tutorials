# LD_LIBRARY_PATH

To define this variable, simply use (on the shell prompt):
```
export LD_LIBRARY_PATH="/path/to/sdk/lib"
```

To make it permanent, you can edit the ldconfig files. First, create a new file such as:
```
sudo vi /etc/ld.so.conf.d/your_lib.conf
```

Second, add the path in the created file
```
/path/to/sdk/lib
```

Finally, run ldconfig to update the cache.
```
sudo ldconfig
```
