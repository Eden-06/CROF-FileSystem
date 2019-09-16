# CROF-FileSystem

Another example for the [CROM-based Modeling Framework](https://github.com/Eden-06/CROF) using a simple FileSystem.
In this example, role-based design patterns should be employed assigning the domain classes to play the appropriate role types from the design pattern, i.e., `Composite` and `Observer`. In detail, this task focuses on a simple *file system*.

> **A *file system* includes *files* and *directories*.
> Both files and directories have a modifiable *name* and return their *size* in Bytes.
> While files return the size of their content, directories should return the accumulated size of all containing directories and files.
> A directory can contain multiple files and directories as children.
> Whenever a file or directory changes it's size, its enclosing directory should be notified to recompute its size.**

The initial CROM model (stored in `model/FileSystem.crom_diagram`) is shown below:

![Initial CROM model from `model/FileSystem.crom_diagram`](https://github.com/Eden-06/CROF-FileSystem/blob/master/model/FileSystem.svg)

# Import into FRaMED 2.0 and Code Generation

1. Import the `CROF-FileSystem` repository into the Eclipse Instance.
    1. Select "File" -> "Import" to open the import wizard, select "Projects from Git" and hit "Next>".
    2. Enter <https://github.com/Eden-06/CROF-FileSystem.git> into the URI field and hit "Next>"
    3. Only select the **master** branch and continue with "Next>"
    4. Continue with "Next>" until you can "Finish" the project import.
2. Open the added `CROF-FileSystem` project and open the model folder.
    * If *FRaMED 2.0* was installed, simply open the `FileSystem.crom_diagram` file by double clicking on it.
    * Otherwise, open the `FileSystem.crom` file directly (double click) in the standard Tree Editor.
3. By left clicking on the `bank.crom` file, and clicking on the context menu entry "Generate > CROM Framework", the framework is tasked to create the model code for the *FileSystem* CROM model.
