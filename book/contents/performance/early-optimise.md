# 糟糕的提前优化


## 函数调用
由于Rust的编译器和LLVM很强大，因此就算你使用了多层函数调用去完成一件事(嵌套函数调用往往出于设计上的考虑)，依然不会有性能上的影响，因为最终生成的机器码会消除这些多余的函数调用。

总之用Rust时，你不必操心多余的函数调用，只要写合理的代码，然后Rust会帮助你运行的更快!