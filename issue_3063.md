
   # Bug Report: Different Output on Running the Same Binary

## Issue Link:
[WasmEdge Issue #3063](https://github.com/WasmEdge/WasmEdge/issues/3063)

![WasmEdge Error Output](/images/issue_3063_1.png)


## Problem Description:
Running the following command throws an error in WasmEdge:
-	Verifying the same with wartime, and warmer outputs

![WasmEdge Error Output](/images/issue_3063_2.png)


```bash
wasmtime --invoke main /root/filea29176_1.wasm 
```



![WasmEdge Error Output](/images/issue_3063_3.png)

```bash
wasmer compile /root/filea29176_1.wasm -o /root/filea29176_1.wasmu
```

![WasmEdge Error Output](/images/issue_3063_4.png)


