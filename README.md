# CROF-FileSystem

Another example for the [CROM-based Modeling Framework](https://github.com/Eden-06/CROF) using a simple FileSystem.
In this example, role-based design patterns should be employed assigning the domain classes to play the appropriate role types from the design pattern, i.e., `Composite` and `Observer`. In detail, this task focuses on a simple *file system*.

> **A *file system* includes *files* and *directories*.
> Both files and directories have a modifiable *name* and return their *size* in Bytes.
> While files return the size of their content, directories should return the accumulated size of all containing directories and files.
> Whenever a file or directory changes it's size, its enclosing directory should be notified to recompute its size.**

The initial CROM model (stored in `model/FileSystem.crom_diagram`) is shown below:

![Initial CROM model from `model/FileSystem.crom_diagram`](https://github.com/Eden-06/CROF-FileSystem/blob/master/model/FileSystem.svg)
