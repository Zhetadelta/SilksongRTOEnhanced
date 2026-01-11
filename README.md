# SilksongRTOSplitsGenerator
LiveSplit splits (.lss) and autosplit configuration generator for Silksong Semirandom Tool Order.

Notable changes from the forked repository include:
- Inclusion of crests and silk skills
- Progression limiting for shorter runs via command line arguments
- Automatic configuration of autosplitter
- Sane generation: tools will generally follow a progression from early to late, with substantial mixing of pools to ensure variety.

How to use:
1. Download the `.exe` to any folder.
2. Double click the `.exe` (or run it with command prompt).
    - Double click will use default settings for the following launch options:
    - "e=long" to disable generation for Egg of Flealia and Throwing Ring. A comma seperated list like `e=long,crest,skill` can be used as an argument.
    - "max=faydown" to disable act 3 tools and items.
3. The program will generate a random list of tools while honoring prerequisites.
4. The LiveSplit file will be saved in the same directory as the .exe to `rto-Tool-Name.lss`. The name will be based on the first tool in the splits. In the event that the filename is identical to another file in the directory, it will overwrite the existing file.
5. This `.lss` file can then be opened by LiveSplit.
