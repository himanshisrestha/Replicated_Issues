
   # Bug Report:Do not terminate while executing the given test case

## Issue Link:
[WasmEdge Issue #2733](https://github.com/WasmEdge/WasmEdge/issues/2733)

![WasmEdge Error Output](/images/issue_2733_1.png)

WasmEdge :

![WasmEdge Error Output](/images/issue_2733_2.png)
![WasmEdge Error Output](/images/issue_2733_3.png)
![WasmEdge Error Output](/images/issue_2733_4.png)

Wasmtime :

Remarks : WasmEdge should throw an error similar to WasmTime stating a misaligned pointer, but it doesnot.





