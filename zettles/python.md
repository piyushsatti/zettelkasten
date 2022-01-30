# Python
> Zettle for everything I find out in Python.

### Module Parent Imports
> You can read more about them [here](https://docs.python.org/3/tutorial/modules.html)
Module imports cannot go to a parent directory. However, in a complex project there is additional caveats. While the project is run from the base directory the file itself may be run from some sub-folder. In such a case, appending the path to the file must be done with respect to the bast directory and not relative to the file position in the project. This is because the pathing of import is taken relative to the file positon but the sys.append method runs from the base directory. In such a case, erro is not thrown and it can be hard to debug.
eg-->

> base -> 
> &emsp;class -> class_ex.py
> &emsp;utils -> run.py

```py
import sys

# doesnt work
import class.class_ex

# doesnt work
sys.append("../")

# works
sys.append(./base)

import class.class_ex

# also better to use
# pathing for cross dependencies
# to make system agnostic
path = os.path.join(os.path.curdir, 'src', 'classes')
sys.path.append(path)
```

### Module imports in complex projects
> This is an important problem and you should read up more on this.
The module import is based on the system path generated from the root file being executed. If you are importing any sub-modules that have their own modules you need to append said paths to the system path so as to execute the code. Otherwise the python program will not be able to find a path to the sub-module being imported (mainly in the case where the the sub-modules reside in different sub directories.)

### Generators
Generators can be creating using yield command in whatever function you want to create. It just acts like a 'stop and do as required command' to stop over consumption of the system resources. However, generators cannot be used again after a **StopIteration** error has been reported by the generator object. One may need to create the generator object again after getting this error if they are to use the generated information again.
