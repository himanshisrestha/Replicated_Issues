
   # Bug:Wasi path_readlink not work well
   ## Issue Link:

[WasmEdge Issue #1993](https://github.com/WasmEdge/WasmEdge/issues/1993)

## Steps to reproduce : 

```
1. Make a directory structure as shown:

root/
├── test.txt
└── test/
    └── test-link.txt -> ../test.txt

```

```
2. Create a symbolic link between them:

ln -s ./test.txt ./test/test-link.txt

```

```
3. Create a rust project directory

Add the test code in src/main.rs 

```

```
4. Build the project and then run using wasmedge 
```

![WasmEdge Error Output](/images/issue_1993_1.png)

Output:
Remark : The issue does exist.
