   # Bug Report:The test case should trigger “misaligned pointer” error, but it return OOB error now
## Issue Link:

[WasmEdge Issue #2881](https://github.com/WasmEdge/WasmEdge/issues/2881)

![WasmEdge Error Output](/images/issue_2881_1.png)

WasmEdge :

![WasmEdge Error Output](/images/issue_2881_2.png)

Wasmtime : 

Remarks :
a. When using the file mutated_file_170.aot.wasm, OOB error is triggered, whereas, on using some other file name , it going to run forever.
b. Wasmedge should throw error here instead of running forever.




