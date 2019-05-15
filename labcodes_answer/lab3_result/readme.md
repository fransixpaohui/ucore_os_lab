## 关键数据结构理解

里面有两个数据结构mm_struct 和 vma_struct

我觉得mm应该就是整个内存空间

vma是一个个虚拟内存区域

mm通过mmap_list作为链表头链接下属的vma

vma通过vm_mm反向连回自己所属的mm


