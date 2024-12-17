# Lua Function Unexpected Nil Return

This repository demonstrates a subtle bug in a Lua function that handles nil arguments. The function `foo` aims to return either `a`, `b`, or their sum, depending on whether the arguments are nil.  However, when both `a` and `b` are nil, it returns nil instead of perhaps a default value (0, for example).

The bug is in the logic of handling nil values.  A more robust solution is provided in `bugSolution.lua`.