traverse
========

Doing science with filesystem traversal!

The `src/` directory in this repository contains two python scripts: `traverse.py` and `traverselite.py`, both of which recursively traverse a filesystem and collect data. `traverse.py` requires some additional Python libraries, including `numpy`, `scipy`, `matplotlib`, and `docopt`, which are not bundled with all Python installs and may not be available on all systems, such as Alden Hall lab computers. Therefore, I've bundled an additional script, `traverselite.py`, which will do data collection and output CSV files (as well as text to the console) without using the data analysis and graphing features provided by those libraries.

If you want to help contribute to my filesystems statistics research project, please download this repository, run `traverselite.py` on your home directory, create a CSV file, make a fork of my repo with your output CSV files in the `data/` directory, and send me a pull request. I'm planning on doing all of my data analysis & graphing in an IPython notebook, which I'll make publicly available once it's complete.

`traverse.py` should run on any computer with a working installation of Python 3 — Windows, Mac, Linux, it doesn't matter. Please collect data from as many computers as you can — your home computer, Alden Hall lab computers, et cetera. Traversal of extremely large filesystem trees may not happen instantaneously: I've seen traversals take as much as 15 seconds, so please give the script a few moments to run. It can be run in verbose mode, where it'll print every file and directory it encounters to the console, which can be used if you want to make sure the script is running and hasn't crashed.

Usage instructions:
--------------------

```
Usage: 
    python traverselite.py (DIRECTORY) [--size] [--links] [--verbose] [--csv]

Arguments:
    DIRECTORY           Root directory from which to begin traversal.

Options:
    --verbose       Verbose mode execution
    --size          Analyze file size
    --links         Analyze file link count
    --csv           Output a CSV
```

If you want to contribute to my research, please run the following command:
```
    python traverse.py ~ --csv
```

Feel free to add the `--verbose`, `--size`, and `--links` flags as well, if you're interested in additional information.

Thanks guys!

 — Hawk (weismanm@allegheny.edu)