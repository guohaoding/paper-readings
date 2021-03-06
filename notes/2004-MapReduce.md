### Goal
解决并行计算的复杂性。
### Problem
需要用大量复杂代码处理如何并行计算、分发数据和处理容错，使得原本简单的计算变得难以处理。
### Solution
设计一个新的抽象模型，使我们可以表达想要执行的简单计算，在库中隐藏了并行化计算、容错、数据分发和负载均衡等复杂细节。
### Contributions
- 抽象出简单而强大的接口可以自动并行和分发大规模计算，结合这个接口的实现可以在大型普通PC集群上实现高性能

### What is MapReduce
MapReduce是一个用于处理和生成大规模数据集的编码模型和相关实现。使用这个编程模型，用户一般只需指定map和reduce两个函数：
- map：处理输入的key/value对并产生一组中间key/value对
- reduce：合并相同中间key的value值并生成一组合并后的value  

MapReduce提供：
- 自动并行化计算和数据分区
- 容错

### Example
- 分布式排序
- 分布式Grep
