
   # Bug:Failed to read the soft file of a source link file
   ## Issue Link:

[WasmEdge Issue #3493](https://github.com/WasmEdge/WasmEdge/issues/3493)

## Steps to reproduce : 
```bash
1. Requirements :

wasi-sdk to compile C code to .wasm
```

```bash
2. Create a test.c file with the following code to test symlinks working or not
```

![WasmEdge Error Output](/images/issue_3493_1.png)

```bash

3. Make a directory structure like this:

subdir_1/
└── subdir_1/
    └── subfile_2
softfile_1 -> subdir_1/subdir_1/subfile_2 (symbolic link)
```
```4. Compile the .c file to .wasm and then use wasmedge to run it.```

![WasmEdge Error Output](/images/issue_3493_2.png)

```
Output:
Remarks :  Both wasmedge and wasmtime produces the same expected result. So the issue is 
```
![WasmEdge Error Output](/images/issue_3493_3.png)

seeming to be invalid here.


