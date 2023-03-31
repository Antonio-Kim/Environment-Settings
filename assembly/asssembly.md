# Assembly (x64)

## Setting gdb to Intel
```bash
echo "set disassembly-flavor intel" > ~/.gdbinit
cat ~/gdbinit
```
After that, when compiling C/C++ codes, add -g flag to have extra information for gdb.
For example, typing "list" will output the code. To find instructions, use
"disassemble main" to get the assembly code.


