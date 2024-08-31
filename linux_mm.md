# struct mm_struct

进程内存描述符，可以理解为虚拟地址块(vma)管理

## 成员
```
struct vm_area_struct *mmap
```
vma的链表头

```
unsigned long rss
```
分配给进程的页框数

