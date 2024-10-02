
   # Bug Report:The result is different from other warm runtimes while executing the given wasm file

## Issue Link:
[WasmEdge Issue #2761](https://github.com/WasmEdge/WasmEdge/issues/2761)

![WasmEdge Error Output](/images/issue_2761_1.png)

WasmEdge :

![WasmEdge Error Output](/images/issue_2761_2.png)

WasmTime :

Remarks : As said in the comments, if we don’t optimise the code using “—optimize 0” then OOB error is thrown , else wasmedge outputs the checksum.

